## https://www.freecodecamp.org/news/react-context-for-beginners/

Sorter way to implement Context API-run in sandbox

import React, { useContext } from "react";

export const UserContext = React.createContext();

export default function App() {
return (
<UserContext.Provider value="Reed">
<User />
</UserContext.Provider>
);
}

function User() {
const value = useContext(UserContext);
return <h1>{value}</h1>;
}

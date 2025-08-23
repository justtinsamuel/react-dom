# react-router-dom
front end

## Setup
npm create vite@latest (folderName) react-router-dom
cd (folderName)
npm i
npm i react-router-dom

cd src
mkdir components pages router
create index.jsx
mkdir layouts
create MainLayout.jsx

cclear app.jsx dan app.css

## Init use router-router-dom
# in app.jsx:
import { RouterProvider } from 'react-router-dom';

in app function:
  <RouterProvider></RouterProvider>

# in MainLayout
import React from "react";
import { Outlet } from "react-router-dom";

const MainLayout = () => {
    return(
        <div>
            <h3>To Do Apps</h3>
            <Outlet></Outlet>
        </div>
    )
} 

remember rafce, for quick import. atau ctrl + space.

Step By Step:
1. router: Index.jsx isi PATH nya.
2. layouts: Create main layout
3. pages: create pages sesuai PATH di router nya.
4. edit app.jsx
5. testing PATH di http://localhost:5173/ (default vite)
6. use tailwindcss npm i -D tailwindcss @tailwindcss/vite (pakai vite)
7. vite.config.js import tailwindcss nya, add plugins.
8. import di index.css
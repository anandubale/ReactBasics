# ReactBasics
Started Learning React and Basics of it

//Basics of JS for React:-

    Functions and Arrow Functions -Done
    Objects
    Arrays and array methods
    Destructuring
    Template literals
    Ternary Operators
    ES Modules and Import / Export Syntax

//Create React app
    npx create-react-app <ProjectName>


//Folder Structure 
Node Modules:-- 
    Dependency Which Get Used in all Projeect dependecies of dependency

public folder:- 
    contains static assets like image/icons and index.html

Index.Html:-
    
    Title 
    Fonts
    css
    favicon
    id="root" -our Entire app

src:- 
    brain of our app
    all work happens here
    js enttry point is in here only src/index.js

.gitignore :-
    select which file source should we ignore for github


package.json:- 

    it contains info about our project like list of dependencies and scripts
      
package-lock.json:-

    it contain snapshot of entire project tree



//Shortcut
Ctrl B => close sidenav bar of Vs code
h2#something.SomeValue  => <h2 id="something" class="somevalue"><h2/>
    snipped shortcut with es7 extension
    rafce(arrow function with export)
    rfce(regular function with export)
    reaxt auton import


####Typical Component ####

1.import (optional)
2.logic(function)
3.export




//E.g


                ```
                function Greeting(){
                    return <h2>My first Component</h2>;
                }

                //Arrow function also Works

                const Greeting= () => {
                    return <h2>My FIrst Component</h2>
                }


                COMPONENT RULES
                Rule no 1:- always start component with capital letter
                Rule no 2:- Always should return JSX
                Rule No 3:- Always Close Tag <Greeting/>

                export default Greeting;
                //with out () this we are not calling it remember 
                //just stating the name

                below Logic if for root Component only (Only One)
                ```

                import React from 'react';
                import ReactDOM from 'react-dom/client';

                const Greeting =()=>{
                    return <h2>My FIrst Component</h2>
                }

                const root = ReactDOM.createRoot(document.getElementById('root'));
                root.render(<Greeting/>);



JSX Started:- 1:12:55 done



#### JSX ####

function + Html


function Greeting(){
    return (
        <h2>Hello World<h2/>
    )

}

Point to Remember:- Return() not return{}


without JSX it code will be like this

function Greeting(){
    return ReactDOM.CreateElement{'h2',{},'Hello World'};
}


Rule1 :- Always return one element from JSX like div/h2/anything bt only one
        //can use one parent to bind multiple child

Note:- Fragment

    Try to make Symantic if u want 
    NON Symantic-Div tag only getting used for all
    Symantic -header footer nav main article section tags getting Used

    if you dont want both then use

    Fragments-allow to group extra element without adding extra nodes

    e.g return <React.Fragement>..rest of Return <React.Fragement/>
                                   or 
        return <>...rest of return </>

Note:- always use camel case like "className"
Note :- Always close every Element or you'll get Error <img/>  <input/>
Note:- if ur not using () then make sure 
        opening tag on same line atleast  return <h2> or 
        whole on same line return <h2></h2>


#### Nested Component ####










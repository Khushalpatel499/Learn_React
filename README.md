# Learn_React

Q.why react needed?
1.react came into 2013. 2. early when we go to an url,backend send the html,css,js file and when a user submit a form we simply send that back to the server t store that information.
3.Now a user simply clicked on the page we simply request a new html file and the new page from the server and that gets sent to the front end that how website work for many years. 4. the problem is that all the website work on the different browser and these browsers are implemented differently. 5. as we use more and more js in our website we have see it work differently for each of browser. 6. eventually to solve this problem we had jQuery come out which allowed developers to esily interect with DOM across all these browsers.Dom display how our page look like and it is a tree like structure. js all do to modify this DOM 7. jQuery made developers happy because it had . unified easy API ,Instead of a developers tryping to think about how to work with the DOM in each of the different browser,jQuery said ,we will take care of that complexity for you. 8.As website size increase libraries like Backbone.Js came out beacuse js file started getting big.so libraries like Backbone js allowed us to organize these js files and became easier.similary with aJax we now has different system we focus more on the js. 9.now we only load the application code once,instead of request each time and load new document now our application acted more like a desktop application we stay on the same page the entire.
and js file simply update or change the html file or DOM to display new things. 10. we were able to sign into an application and interact with that application without ever speaking to server will became more popular. so in 2010 AngularJs which is created by google popular , now Angular allowed developers to build these large application by forming these .containers that will wrap your project 11. NOw had better containers controllers,views,models and this idea of a model view controller where each part of the application or each js file divided into different things. 12. As think started getting more and more complex beacuse of this as thing get bigger and bigger, user get click on these button to change this area and that button to change that area and so on. it increase the code complexity which it getting harder and harder to find the bugs in the code and data was flowing everywhere. 13.so facebook came up with a solution in 2013 and realease the react.

// NOw the succes of react come up with the four key things

1. Don't touch the DOM . I will do it.

before many exisiting frameworks and librararies before React where directly manipulating the Dom.

DOM: it is a basically browsers uses to display a web site or a web app and js simply manipulating it
this way of manipulaating directly is called imperative.(The problem with imperative approach is that it see difficult relationship between events and there edge cases)

so react came up with a more declarative approach with a novel concept that DOm manipulation is one of the biggest performance bottlenecks, it takes a long time for DOM changes to happen, The browser has to do two really intensive operations
1.repaint: change an element and added onto a page and then refloat which is to recalulate the layout of the page and move things around .
so react says hey you know what lets me take care that i will find the best way for me to change the DOM and just dealcre to me what your app looks like.

so all we need to do is to that this is a js object of how i want the app to look and react is going to hold this js object this massive blue print of how things should look.
so we have to accounted all states in one place, that is one big js object that describe how our app should look. this give a less complexity , better code quality and faster developers times.

so base on the whaterver state or data i am going to react to it and so get the display that you want that's why it name is react.

2.Build websites like lego blocks

it use the idea of reusable components
react use that small components that we put them together to form bigger components,and component containing components just lik lego blocks.
so these components can use in different places. or different project to reuse them.
so we can build these components like material UI components ,different component libraries like ReactBootstrap, or blueprints.
in simple term it is just plain js function that we write
components are created on the base of data or state well simply a function
so components are simply just js functions that receives some sort of input or attributes which we called props and in return it returns this things that kind of look like html but inside js.
this component can be built like function or even as a class.
but the key here is that based on the state and these components that we built , we have entire component that we can add to our page and reuse it.

in browser react pulg in allow us to see the component that we built into application.

3.Unidirectional data flow

the idea of state which is the data of our app , work with the components which are built using
called jsx(it is html like syntax inside of javascript)

this all combine give our react libraray two thinks
that is the component that we have built, the state of our application we can think of this as a function.
A React library is simply a function that we give all these things, it going to do that it create what we call a virtual dom, that is it create a js version of dom
virtual dom is a tree like object that give react a blueprint that how it should update the acutual dom.
so what happen then react takes all of this and says here is the actual dom
unidirectional data flow means that any time we want something to change on our web page well the state has to change that is the data has to change in our app,as soon as it going to trickle down that information and let everyone know hey the state just changed.
restriction of data only being able to move down from
the state of application all the way to the dom.
and change to state we go to state and the state change tricle down to different component.
it is very easy to debugg our code.

4.I am just UI, the rest is up to you

as we see angular is kind of framework which is like a whole kitchen , it gives the developers all the tools neccessary to build an application
but react said i only care about this whole idea of components and virtual dom and only going to work with the view , the user interface everything else that you need ,well you can just use other modules , other libraries and mix and match and have whatever you want customized to your need.

so it was a library , a UI library which is not like a kitchen, like a stove they gave you the stove to cook your soup on ,but everythink else like knife cutting,bord ,spoon other which ever you want to pick is up to you what you use to build that soup.

the key idea becuase it was so small you can learn once and write everywhere means react doesn't make assumption what technology stack you use

all it give you is here is this idea of components of a blueprint that we can use a massive js object to make change and here is also a robot that well interact with the dom and make changes for you, it only focuses with the UI, we are able to move react to other places othan than web, we have now different robots that interact with different views and they need is this main react library or blue print of how to well look at a js object and change the UI.

so now we have things like React native this other little robot can look at this blueprint and this change the view in a ios or android app. although it might not know anything about the dom,it only need to know about views in a mobile app.

we also have React 360 which is using the blueprint and use in VR apps, this little robot or library can focus on VR.

we also have Electron and React Desktop that allows us to build desktop appliction, they interact with windows ,Mac and Linux operating system.
we also have React Blast that work with the Terminal and the command prompt.

THis idea of cross paltform really took off with React.
when we do our project we import two libraries the core React Library, which is this little robot and the React DOM library which is this specific robot that onnly know how to interact with the DOM or the web Browser

so now react like concpet update in angular, vue use by developers to build the front end appliction.
but react is still most popular library.

some important react words.

Declarative, JSX, Components, State, Props, Virtual DOM

Declarative: instead of telling our app what to do we simply give our it some state , some components that are built with something called gsx and these components sometimes receive properties which are called props, we give all that information a gaint js object in a declarative way, which creates a virtual DOM in js, that virtual dom is used by the react library to update the DOM for us in a declarative way.

how to become best react developers?
1.Decide on Components
2.Decide the state and where it lives 3. What changes when state changes.

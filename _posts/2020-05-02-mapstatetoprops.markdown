---
layout: post
title:      "mapStateToProps?"
date:       2020-05-02 10:19:59 +0000
permalink:  mapstatetoprops
---


A key component of being my journey of being able to understand Redux better was first understanding the functions mapStateToProps and mapDispatchToProp, because one would need to understand what happens here before being able to incorporate these within our components or manipulate state successfully. 

Firstly, it was important for me to clearly distinguish once more the difference between props and state in React, otherwise, putting them in the same line as a function "map**State**To**Props**" can definitely throw anyone off a bit. So in a knutshell, the key difference between props and state would be that props are data or variables passed to a child component by it's parent component, meanwhile state on the other hand are directly initialized and managed by the component. The state can be initialized by props and the state can be later passed down props to another component. Props are also never changed within a child component. 

With that being said, using Redux, our mapStateToProps function would work alongside the **connect** function that redux provides as well. So connect is synced to our redux store, it listens to any change that occurs in the redux store state and it then calls this magical function of mapStateToProps - This is where we would specifiy which part of that state, if not everything, that we would want to send to our component as props for that compenent. An example would be connect(mapStateToProps)(componentName) which would typically be in a component that we would export!

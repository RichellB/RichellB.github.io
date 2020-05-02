---
layout: post
title:      "Understanding Redux"
date:       2020-05-02 10:00:01 +0000
permalink:  understanding_redux
---


Being introduced to React definitely takes one's programming mindset to another world but incorporating Redux, althout it may seem complex at first, has defiitely made everything with React so much easier, quicker, with more organized code Using Redux allows us to create a globally available state to replace having to pass down our data as props, particulary to numerous children components. A little summary of my understanding of Redux would be:

To begin, Redux has three main principles to always keep in mind:
* Single source of truth : This means that it should be the same Redux store state that is accessed and we can make copies of this if needed!
* State is read-only: Now state has to be ready only, meaning we would never directly alter the state within the Redux store. However, changes need to be made to the state of course, which brings us to the third concept
* Changes using Pure Functions: these changes to our state should be done with pure functions (Pure functions are essentially functions that have no side effect to our app, that is,  it always should have the same output if it is given the same input).

Using React-Redux, it provides us with a Provider, which generally ensures that our app can potentially access the state from the store. So we wrap the Provider around our App component and it then does two key functions: it alerts our Redux app whenever there's been a change in state and it would then re-render our React app. So how will these two functionalities be carried out? 

There would be a few features that we need to incorporate here to get this done, but it will all be worth it in the end! These features include setting up our createStore function, reducers, actions, mapStateToProps, mapDispatchToProps/our dispatch function(s), and also using our connect function to wrap everything together with our components. 


![](https://www.google.com/search?q=redux+images&sxsrf=ALeKk02Pv2t3FQ7mLvT1c11WbQ7FP4zeAw:1588413363928&source=lnms&tbm=isch&sa=X&ved=2ahUKEwj7zMDy9JTpAhWQlnIEHRc7AjQQ_AUoAXoECBIQAw&biw=1366&bih=625#imgrc=KcJnm65zQBehPM)

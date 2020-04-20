1. What problem does the context API help solve?

It provides a way to share values between components without having to explicitly pass a prop through every level of the tree.

1. In your own words, describe `actions`, `reducers` and the `store` and their role in Redux. What does each piece do? Why is the store known as a 'single source of truth' in a redux application?

actions - are payloads of information that send data from the app to the store.

reducers - specify *how* the application's state changes  due to what the actions sent to the store. they only descripe *what happend*.

store - holds the whole state tree of the application. This shouldn't be confused with a class. It's just an object with some methods on it. The only way to change the state inside, is to dispatch an action on it.

1. What is the difference between Application state and Component state? When would be a good time to use one over the other?

Application State is the global state that *ALL* the components in the component tree can access. It is also Immutable.
Components State is the state that is local to a single component and can't be seen outside of that component. It is a mutable state so you can change the state when you need to.

1. Describe `redux-thunk`, what does it allow us to do? How does it change our `action-creators`?

Redux Thunk is a middleware that provides the ability to handle asynchronous operations inside of your Action Creators.

1. What is your favorite state management system you've learned and this sprint? Please explain why!


I think Context API because it's a lot less verbous and more conveninet to implement.

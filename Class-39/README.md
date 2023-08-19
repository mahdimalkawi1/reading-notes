# Read: Class 38

## React 3:

### Q1. What is React Context, and how does it help in managing state and data sharing in a React application?

React Context is a feature that helps in sharing data (like state, settings, or user information) across components without manually passing props. It creates a central store of data, and components can access this data from anywhere in the component tree. This reduces "prop drilling" and simplifies data sharing. You create a context using React.createContext() and wrap components with a Context.Provider to make the data available. Components then use the useContext hook to consume the data. While Context is useful for simpler cases, more complex apps might benefit from other state management libraries like Redux for advanced scenarios.




### Q2. Explain the useContext Hook and how it can be used to access data from a React Context within a functional component.

The useContext hook in React lets functional components access data from a Context. First, create a Context with React.createContext(). Wrap your components with Context.Provider to provide the data. Then, use useContext(MyContext) to retrieve the data in your functional component. This avoids prop drilling and simplifies data sharing.




### Q3. Describe the purpose of Next.js, and provide an example from the Vercel Next.js Examples reading on how it can be used to build a scalable web application.

Next.js is a framework for building web apps with React. An example is creating a blog. You organize pages in the pages folder. Data is fetched using getStaticProps or getServerSideProps. Dynamic routing renders individual blog posts, enhancing SEO. Navigation uses Next.js's Link component. Styling and components are flexible. Vercel simplifies deployment, optimizing performance. Next.js streamlines building web apps with React, aiding in SEO, routing, and deployment.





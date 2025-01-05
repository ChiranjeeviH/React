# React
React Fundamentals learning
# Why React
1) Component-Based architecture
2) Virtual DOM
3) Declarative syntax
4) Reusability
5) EcoSystem backed by strong community

# Things to learn
1) Component Architecture
2) Lists and Forms in React
3) Fetch Real-time data from external API's
4) Add features - Search, Sort, Filter, Local Storage
5) Deploy using Netlify
6) Prop Drilling and Context API
7) React Hooks
8) Project and Interview Prep

# Way of Rendering (HTML,Plain JavaScript, React using CDN's)
# HTML:
<div id="root">
    <h1>Hello World</h1>
</div>

# JS
 <script> 
        const messge = document.createElement('h1')
        messge.innerHTML = "Hello World from JavaScript"
        const root = document.getElementById("root")
        root.appendChild(messge)
 </script>
    
# React using CDN's
<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
 <script>
        const message = React.createElement('h1',{},'Hello World from React')
        const root = ReactDOM.createRoot(document.getElementById('root'))
        root.render(message)
 </script>
  <!-- HTML way of writing Parent and child elements
          <div id="parent">
            <div id="child">
                <h1 id="greeting">Greeting</h1>
                <h2 id="greeting1">Greeting1</h2>
            </div>
         </div>

          <script>
            <!-- React way of writing the above HTML parent and child cases with the help of CDN's-->

            const message = React.createElement('h3', {}, 'Hello World from React')

            const greetings = React.createElement('div', { id: "parent" }, React.createElement('div', { id: "child" }, [React.createElement('h1', { id: "greeting" }, "Greeting1"),                 React.createElement('h2', { id: "greeting1" }, "Greeting2")]))

            const root = ReactDOM.createRoot(document.getElementById('root'))

            root.render([message, greetings])

        </script>

# Create React project with the help of Vite
1) npm create vite@latest
2) npm install (inside the the newly created project)
3) npm run dev
Single command
npm init vite@latest my-app --template react

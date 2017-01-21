# todo_react_tutorial
Ref from kirupa.com https://www.kirupa.com/react/simple_todo_app_react.htm


React terminology and Key concepts

Framework for creating Views using reusable components.
Uses Virtual DOM for effective and precise rendering of changes.

React and ReactDom 
Including React in project 1) CDN url 2) npm

Components : Stateless pure functional components, Container components with state.
State is used for things that have to change for a component when things like hover, onclick etc happen.
When props are used the properties of the component are passed during component creation and as long the component lives in browser memory.
Use state when things for a component have to change, use props otherwise
Children: different from both state and props 
               var Component = React.createClass({

                render: function() {
                     return(
                            <div>
                                 <h3>{this.props.user}</h3>
                                 <p>{this.props.children}</p>
                            </div>
                     );
                  }
               });


             ReactDom.render(
                    <Component user="ABC">This guy is ABC</Component>
               <Component user="XYZ">This girl is XYZ</Component>
,
                     document.getElementById('content')
             );

       -   Refs : Way to uniquely identify/modify elements within a component
         https://facebook.github.io/react/docs/refs-and-the-dom.html
 React.PropTypes
      https://facebook.github.io/react/docs/typechecking-with-proptypes.html
Contexts 
https://blog.jscrambler.com/react-js-communication-between-components-with-contexts/


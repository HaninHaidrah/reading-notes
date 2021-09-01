## Qusetions about React Docs - Forms:  
1. What is a ‘Controlled Component’?
* It is An input form element whose value is controlled by React .  
!(comp)[https://www.bram.us/wordpress/wp-content/uploads/2020/03/uncontrolled-forms-name-attrs.png]
2. Should we wait to store the users responses from the form into state when they submit  the form OR should we update the state with their responses as soon as they enter them? Why.  
* store them then update to be rendered   
### “how to store input from a input field to state in react” Code...
1. > class NameForm extends React. Component {
     constructor(props) {
      super(props);
     this. state = {value: ''};
     this. handleChange = this. handleChange. bind(this);
     this. handleSubmit = this. handleSubmit. bind(this);
      }  


3. How do we target what the user is entering if we have an event handler on an input field?   
* to target the inputs we use this code as an ***example***
![code](https://www.codegrepper.com/codeimages/event.target.name-react-submit.png)  




## Questions about The Conditional (Ternary) Operator Explained:
1. Why would we use a ternary operator?
* its a shorthand write of if statement in react . The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark (?), then an expression to execute if the condition is truthy followed by a colon (:), and finally the expression to execute if the condition is falsy. This operator is frequently used as a shortcut for the if statement.    
!(code)[https://www.codegrepper.com/codeimages/javascript-ternary-operator.png]  

* sntax code :
  > condition ? value if true : value if false


2. Rewrite the following statement using a ternary statement
  >condition ? value if true : value if false
  >    > (x===y)?  console.log(true): console.log(false);

 
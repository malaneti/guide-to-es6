# guide-to-es6

Key Features in ES6


1)Arrow functions – A short-hand version of an anonymous function.
    
    -simplify function scoping and the this keyword
    -avoid having to type the function keyword, return keyword (it’s implicit in arrow functions), and curly brackets.
    -Because arrow functions allow you to retain the scope of the caller inside the function, you don’t need to create self =     this closures or use bind.
    


    ex: var multiply = (x, y) => x*y;
    ex: smartPhones.map(smartPhone=>smartPhone.price)
    ex: 
    // Manually bind, wherever you need to
    class PostInfo extends React.Component {
      constructor(props) {
        super(props);
        // Manually bind this method to the component instance...
        this.handleOptionsButtonClick = this.handleOptionsButtonClick.bind(this);
      }
      handleOptionsButtonClick(e) {
        // ...to ensure that 'this' refers to the component instance here.
        this.setState({showOptionsModal: true});
      }
    }


2)Block-level scope – ES6 now supports scoping variables to blocks (if, for, while, etc.) using the let keyword.

    ex: use let instead of var 

3)Classes – ES6 classes provide a way to encapsulate and extend code.

    ex: class Photo extends React.Component {
    render() {
    return <img alt={this.props.caption} src={this.props.src} />;
  }
}

4)Constants – You can now define constants in ES6 code using the const keyword.

5)Default parameters – Ever wished that a function parameter could be assigned a default value? You can do that now in ES6.

6)Destructuring – A succinct and flexible way to assign values from arrays or objects into variables.

7)Generators – Specialized functions that create iterators using function* and the yield keyword.

8)Map – Dictionary type object that can be used to store key/value pairs.

9)Modules – Provides a modular way of organizing and loading code.

10)Promises – Used with async operations.

11)Rest parameters – Replaces the need for using arguments to access functions arguments. Allows you to get to an array representing “the rest of the parameters”.

12)Set – A collection object that can be used to store a list of data values.

13)Template Strings – Clean way to build up string values.

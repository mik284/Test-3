
## Take-Away Assessment 

Rewrite this React class Based component into a react functional component 

import React, {Component } from 'react' 

 

export default class Post extends Component { 

 

    state= { 

        posts:[], 

        id:'2' 

    } 

 

    componentDidMount(){ 

        this.fetchPost() 

      

    } 

 

    componentDidUpdate(prevprops, prevstate){ 

        if(prevstate.id!== this.state.id){ 

            this.fetchPost() 

        } 

    } 

 

    async fetchPost(){ 

        const response= await fetch(`https://jsonplaceholder.typicode.com/comments?postId=${this.state.id}`) 

        const data= await response.json() 

        this.setState({posts:data}) 

            

    } 

 

  render() { 

    return ( 

        

      <div> 

         <input type="text" value={this.state.id}  

         onChange={(e)=>this.setState({id:e.target.value})} /> 

         <p>{JSON.stringify(this.state.posts)}</p> 

      </div> 

    ) 

  } 

} 

 

Write a code that does the following: Using a prompt allow user to enter numbers separated by commas and print out the sum of the numbers. 

Name two hooks that help in optimizing performance of a react app explain how they help in improving performance. Write code to prove this. 

Why did we move from Context API to Redux? 

Why Did we move from react-redux to Redux Toolkit 

 

JavaScript 

leUsing a Prompt allow user to enter numbers separated by commas the printout the sum of the numbers 

 

Explain this code what it logs and why? 

f 

 

 PALINDROME –A palindrome is a word, number, phrase, or other sequence of characters which reads the same backward as forward 
Write a program that checks whether a word or a phrase is a palindrome or not. 
Examples of a palindrome 
(race car) 

 

General Question 

 

How would you implement a Loging functionality that only logs in users saved in the database? (Explain no code) 

 

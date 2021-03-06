import React, { Component } from 'react'

export class Greet extends Component {
        constructor(props) {
                super(props)
        
                this.state = {
                       count :0,
                     
                       
                };
                
        
                
        }
        increment(){
                this.setState({
                        count:this.state.count+1
                     
                });
               
        }
        decrement(){
                this.setState({
                        count:this.state.count -1
                });
                console.log(this.state.count)
        }
        


                       eventHandler=()=>{
                                this.setState({

                                    value :this.state.count    
                                
                                
                                });   

            
        }
   
      
      
        
        render() {
                
                return (
                        <div><div>
                                  count-({this.state.count})
                                 
                                  </div>
                              
                                <button onClick={()=>{this.increment()}}>increment</button>
                        
                               <span>
                                <button onClick={()=>{this.decrement()}}>decrement</button>
                                </span>
                                <div><div>
                                  
                                  </div>
                                  <div>
                                  <input type ="text" value={this.state.value} ></input>  
                                </div>  
                                <div>
                                <button onClick={()=>{this.eventHandler()}} >click</button>
                                </div>
                        </div>
                               
                        </div>
                )
        }
}

export default Greet


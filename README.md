# Stack in Javascript
Question : How To Push,Pop and Top in the stack
function stack(input){// It is Input Program
    input=input.trim().split("\n")
    let tc=+input[0]
    let line=1;
    let stack=[];// it is empty stack
    for(let i=0;i<tc;i++){
        let arr=input[line++].trim().split(" ").map(Number);
        //console.log(arr)
        if(arr[0]==1){
            stack.push(arr[1])
        }
        else if(arr[0]==2){
            stack.pop();
        }
        else {
            if(stack.length==0){
                console.log("Empty!")
            }else {
                console.log(stack[stack.length-1])// for top element
            }
        }
    }
  }

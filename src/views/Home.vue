<template>
  <div class="home">

<h1 class="heading1">About</h1>
	<div class="intro" id="intro">
		<p class="aside"> Halzo which means “Get It done in Spanish” is a task scheduling 
      and motivation app that reminds you of the daily to-do tasks and provides motivation 
      to do the tasks that you are less willing to do, such as exercise,wake up, read, code
       and so much more.	</p> <br/>
 <figure><img alt="Halzo proto" src="../assets/looks.png" width="600px">  </figure> <br/>

      <h2 class="heading2">Features</h2>
       <div>
       <p>Alarm which tells the user of the task by ringing and saying the user's name,the 
         task which the user scheduled and a motivation word to encourage the user. 
         E.g Hey John,”All progress takes place outside the comfort zone” it's time 
         for you to do your task “ resume 100 days of code.
  </p>      
   </div>

   <figure><img alt="Halzo pix" src="../assets/add.png" width="600px">  </figure> <br/>
   

<h1 class="heading1">Values</h1>
<p>Helps you manage your time by allowing you to lay out what you need to accomplish and 
  then coordinate your time from there. When you first compose it, you'll note the most 
  important tasks and make time for them. You can also see if certain tasks can be easily 
  coordinated.</p>
    <h3>Creator: <a href="https://www.instagram.com/the_coderboy/" target="blank">The_coderboy</a></h3>

  </div>
  </div>
  
</template>

<script>

export default {
  name: 'Home',
  components: {
    
  }
}
</script>


<style  scoped>
.heading1{
color: #000;	
border-bottom: 2px solid #E44232;
width: 80px;
margin-bottom:20px; 
margin-left: 50px; 
}
.heading2{
color: #000;	
border-bottom: 2px solid #E44232;
width: 100px;
margin:20px auto; 
margin-left: 50px; 
}

.intro{
  text-align: center;
}


.home{
  display: grid;
  margin: 100px auto;
  /* grid-gap: 10px 50px; */
  grid-template-columns: 3fr 12fr 5fr;
}
.home > *{
  grid-column: 2/ span 1;
}

.home >figure{
  margin: 0;
  grid-column: 1/ -1;
}
.home{
  font-family: Cambria, Cochin, Georgia, 'Times New Roman', Times, serif;;
}

  p {
      line-height: 1.8;
    }
    a{
      text-decoration: none;
      color: #E44232;
    }
    h3{
      padding: 50px;
      float: right;
    }
</style>

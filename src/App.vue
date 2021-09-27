<template>
<BlogIndex/>
</template>

<script>
import BlogIndex from "./components/BlogIndex.vue"

export default {
   components: {
    BlogIndex
  }
}
</script>

<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-size: 18px;
    font-family: '宋体';
}
*::before{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
*::after{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

ul li {
    list-style: none;
}
a{
    text-decoration: none;
    color: black;
}
a:hover{
    color: cadetblue;
}

body{
    margin: auto;
    display: flex;
    flex-flow: column;
}
header{
    display: flex;
    width: 80%;
    margin: auto;
    padding: 15px;

}
header>nav{
    width: 100%;
    
}
header>.LingBlog-headerIcon{
    padding-left: 50px;
}
header > nav > ul{
    display: flex;
    justify-content: flex-end;
    padding-right: 50px;

}
header >nav >ul>li{
    padding-right: 50px;
}

main{
    width: 80%;
    /* border: 1px solid green; */
    margin: auto;
    margin-top: 60px;
    display: flex;
    flex-flow: row;
    padding:0 100px;
    max-height: 90%;
}
main > .LingBlog-aside{
    display: flex;
    box-shadow: 0px 0px 2px 2px #f4f4f4;
    flex-flow: column;
    justify-content: center;
    align-items: flex-start;
    max-width: 250px;
    margin-right: 20px;
   
    
}
main > .LingBlog-aside>.asideContent{
  
   margin: 0 30px;
   
    
}
main > .LingBlog-aside>.asideContent>.aside-icon{
    margin-top: 40px;
    border: 1px solid #fff;
    border-radius: 50%;
    box-shadow: 0px 0px 2px 2px #f4f4f4;
    width: 100px;
    height: 100px;
    text-align: center;
    margin-bottom: 40px;

}
main > .LingBlog-aside>.asideContent>.aside-name{
    padding-bottom: 10px;

}
main > .LingBlog-aside>.asideContent>.aside-year{
    padding-bottom: 10px;

}
main > .LingBlog-aside>.asideContent>.aside-phone{
    padding-bottom: 10px;

}
main > .LingBlog-section{
    box-shadow: 0px 0px 1px 1px #eee;
    flex-grow: 3;
    margin-left: 30px;
    max-width: 70%;
}
main > .LingBlog-section>ol{
    margin: 10px 40px;
    counter-reset: section;             
   list-style-type: none;
    
}
main > .LingBlog-section>ol>li::before{
    counter-increment: section;  
    content:  counter(section) ": "; 
    flex-grow: 0.5;
}
main > .LingBlog-section>ol>li{
    padding: 4px 4px;
    display: flex;
    justify-content: space-between;
    
}
main > .LingBlog-section>ol>li>.article-list{
   flex-grow: 16;
}
main > .LingBlog-section>ol>li>.article-date{
    flex-grow: 1;
    color: slategrey;
    
}

footer{
    /* border: 1px solid black; */
}
</style>

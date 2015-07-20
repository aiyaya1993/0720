# 0720
JavaScript面向对象的实现
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="author" content="aiyaya">
  	<title>未命名</title>
  	<script type="text/javascript">
  	  /*工厂模式*/
  	  function createBlog(name,url){
  	  	var o=new Object();
  	  	o.name=name;
  	  	o.url=url;
  	  	return o;
  	  }
  	  var myBlog=createBlog("aiyaya","http://www.aiyaya.163.blog");
  	  /*构造函数模式*/
  	  function Fruit(name,price){
  	  	this.name=name;
  	  	this.price=price;
      }
      var like=new Fruit("apple",5);
      /*原型模式*/
      function Animal(name,age){
      	Animal.prototype.name="monkey";
      	Animal.prototype.age=3;
      }
      var Animal1=new Animal();
      /*混合模式*/
      function person(name,age,school){
      	this.name=name;
      	this.age=age;
      	this.school=school;
      }/*构造函数来提供属性*/
    person.prototype.say=function(){
    	alert (this.name+" is "+this.age+" years old");
    }
    var xiaoming=new person("xiaoming",23,"HDU");

  	</script>
  </head>
  <body>
  </body>
  </script>
  </head>
  </html>

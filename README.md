# EJERCICIO-MUMUKI

<pre><code>
object play{

  method jugabilidad(){
    return 10
  }
  method usar(){
    
  }
}
  
object portatil{
  var jugabilidad=8
  var usos=0
  
  method bateriaBaja(){
    jugabilidad=1
  }
  
  method jugabilidad(){
    return jugabilidad
  }
  
  method usar(){
       portatil.bateriaBaja()  
  }  
}

object delfina{
  var diversion=0
  var consola=play
  
  method agarrar(consola){
    consola.usar()
  }
  
  method jugar(videojuego){
  diversion=self.diversion()+videojuego.diversion()
  }
  
  method diversion(){
    return diversion 
  }
  
 }
 
 object mario{
  var diversion=100
  
  method diversionConsola(consola){
  
  if(consola.jugabilidad()>5) diversion=100 else diversion=15}
  
  method diversion(){
    return diversion
  }
 }
 
 object arkanoid{
 
  method diversion(){
    return 50
  }
 }
 
 object pokemon{
    var consola=play
    var diversion=10
    
    method diversionConsola(consola){
        diversion=consola.jugabilidad()
    }
   
   method diversion(){
    return diversion*10
   }
 }
<code></pre>

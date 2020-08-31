<!-- Autor: Alejandro Viloria -->			

<!-- ETIQUETAS DE DATOS GLOBALES EN BLOGGER --> 

<img expr:src='data:post.firstImageUrl'/> <!-- Primera imagen de la entrada -->	
<img expr:src='data:post.featuredImage'/> <!-- Primera imagen de la entrada canvas.xml v1.9.0 -->	
<expr:alt='data:post.title'/> <!-- Etiqueta ALT para imagenes -->
<data:post.author/>	<!-- Nombre del autor -->	
<data:post.authorProfileUrl/>	<!-- Url del perfil de Blogger o Google+ -->	
<a expr:href='data:post.url' style='color:#fff'></a> <!-- URL hacia la entrada -->	
<data:post.title/> <!-- Título de la entrada -->	
<data:post.date/> <!-- Fecha en el formato configurado -->
<data:post.timestamp/> <!-- Fecha y hora de las entradas en el formato configurado -->
<a expr:href='data:blog.homepageUrl'></a> <!-- URL de la página principal. -->	
<data:blog.title/>	<!-- Título del blog -->
<b:eval expr='data:post.longSnippet snippet {length: 150}'/> <!-- Resumen de la entrada. Máximo 1000 caracteres. No interpreta html -->
<data:post.body/> <!-- Contenido de la entrada. Interpreta Html. -->	
<b:section id='sidebar'> </b:section> <!-- Crear sección sidebar. -->
<data:post.numComments/> <!-- Muestra la cantidad de comentarios. -->
<a expr:href='data:post.addCommentUrl' expr:onclick='data:post.addCommentOnclick'><data:post.numComments/> Comentarios</a> <!-- Enlace hacia los comentarios.. -->
<a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
 <data:post.numberOfComments/> Comentarios</a> <!-- Enlace hacia los comentarios canvas.xml v1.9.0 -->
<b:loop values='data:post.labels' var='label'><a expr:href='data:label.url'><data:label.name/></a></b:loop> <!-- Muestra variable label expresada en un bucle. -->
<data:blog.metaDescription/> <!-- Muestra la meta descripcion de la página o del post. -->
<form expr:action='data:blog.searchUrl'> <!-- Ejecuta el enlace de la pagina de busqueda. -->
<input name='q' expr:value='data:view.isSearch ? data:view.search.query.escaped : &quot;&quot;' /> <!-- Devuelve la busqueda en el blog. -->
<input expr:value='data:messages.search'/> <!-- Muestra el boton "Buscar". -->
<URL-de-mi-blog/search?max-results=1000> <!-- Muestra la página de resultados para las busquedas". -->
<expr:style='&quot;background-image: url(&quot; + data:blog.postImageUrl + &quot;);&quot;'/> <!-- Muestra la primera imagen del post como background -->	
	

	

<!-- CONDICIONALES DE BLOGGER --> 

<b:if cond='data:blog.homepageUrl == data:blog.url'> <!-- Mostrar gadgets solo en la portada -->	
<b:if cond='data:blog.pageType == &quot;item&quot;'> <!-- Ejecutar un elemento sólo en las entradas individuales -->
<b:if cond='data:blog.pageType == &quot;archive&quot;'> <!-- Ejecutar un elemento en las páginas del archivo -->
<b:if cond='data:blog.pageType == &quot;static_page&quot;'> <!-- Ejecutar elemento en las páginas estáticas -->  
<b:if cond='data:blog.url == &quot;URL de la entrada o etiqueta&quot;'>  <!-- Ejecutar elemento en una entrada específica o etiqueta específica -->
<b:if cond='data:blog.url != data:blog.homepageUrl'> <!-- Ejecutar un elemento en todas las páginas MENOS en la portada del blog --> 
<b:if cond='data:blog.pageType != &quot;item&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las entradas individuales -->
<b:if cond='data:blog.pageType != &quot;archive&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las páginas del archivo del blog -->   
<b:if cond='data:blog.pageType != &quot;static_page&quot;'> <!-- Ejecutar elemento en todas las páginas MENOS en las páginas estáticas -->   
<b:if cond='data:blog.url != &quot;URL de la entrada o etiqueta&quot;'> <!-- Ejecutar  en todas las páginas MENOS en una entrada específica o etiqueta específica -->   
<b:if cond='data:view.isError'><!-- url no existe muestra la pagina de error 404-->
<b:else/> <!-- casos contrario muestra el blog-->
</b:if> <!-- Cierre de la condicional -->
<b:attr cond='not data:view.isPreview' name='target' value='_top'/> <!-- Condición que indica que no es una vista previa. -->
<b:if cond='data:view.isSearch'> <!-- Mostrar gadgets solo en la página de resutados para la busqueda -->

 
<!-- CSS COMENTARIOS BLOGGER -->
 
/**fix comment**/
.comments .comments-content .loadmore.loaded{max-height:0;opacity:0;overflow:hidden;display:none}.comments .comments-content .comment-thread ol{list-style-type:none;padding:0;text-align:left}

.comments .comment-block {
    margin: 0 0 0 100px;
    color: #777;
    line-height: 1.6;
    position: relative;
}
.avatar-image-container {
    box-shadow: 0 2px 2px -2px rgba(0,0,0,0.2), 0 0 2px 0 rgba(0,0,0,0.1);
    float: left;
    height: 80px;
    overflow: hidden;
    position: relative;
    width: 80px;
    margin-top: 1rem;
    background-origin: border-box;
    background-size: cover;
}

.avatar-image-container > img {
    width: 100%;
    border-radius: 10px;

}
.comment-replies .avatar-image-container {
    width: 38px;
    height: 38px;
    border-radius: 4px;
}
.continue,.item-control{display:none}.comments .comments-replybox{border:medium none;height:250px;width:100%}.comments .comment-replybox-single{margin-left:100px;margin-top:0}
.comments .comment-replybox-thread, .comment-form {
	max-height: 280px;
}
.comments .thread-chrome.thread-collapsed{display:none}.comment-header .user,.comment-header .user a{font-style:normal;font-weight:700;color:#555}.comment-header .user{margin-right:4px}.avatar-image-container img[src="https://img1.blogblog.com/img/anon36.png"],.avatar-image-container img[src="https://img2.blogblog.com/img/b36-rounded.png"]{opacity:0}
li.comment {
    position: relative;
    margin: 1rem 0 1rem 0;
}
.comments-content{}
/**fin fix**/
/**CSS COMENTARIOS**/
/*Defaul CSS Comment v1.0.1*/
.comment {
    position: relative;
}
.comment-replies .comment, 
.comment-replybox-single,
.comment-replybox-thread {
    margin-left: 5rem;
}
.comment-thread ol,
.comment-thread li {
    list-style-type: none;
    text-align: left;
}
.comment-thread ol {
    padding: 0;
}
.comment-thread li::after {
    content: "";
    clear: both;
    display: block;
}
.comment-block {
    margin-bottom: 1rem;
    margin-left: 5rem;
}
.comment-header .user {
    margin-right: .2rem;
}
.comment-header .user, .comment-header .user a {
    font-size: 1.2em;
    color: #333333;
    text-align: left;
    margin: 0;
    font-weight: 400;
    font-style: normal;
    line-height: 1;
}
.comment-header .datetime > a {
    color: rgba(0, 0, 0, 0.4);
    font-weight: 400;
    display: none;
}
.comment-replies .comment-block {
    margin-left: 4rem;
}
.avatar-image-container {
    background-size: cover;
    background-color: #ffffff;
    float: left;
    height: 70px;
    width: 70px;
    margin: 5px 0 0;
}
.avatar-image-container img {
    width: 100%;
}
.comment-replies .avatar-image-container {
    width: 50px;
    height: 50px;
}
.thread-toggle {
    position: absolute;
    right: 1rem;
    top: 1rem;
    z-index: 40;
    display: none;
}
.thread-toggle a {
    text-indent: -9999px;
    display: block;
    width: 20px;
    height: 20px;
    position: relative;
    opacity: 0.5;
    background: url(https://2.bp.blogspot.com/-a8T9QoRSEhQ/WX-4kAduIeI/AAAAAAAACzE/iT_yTwN8Jn8Y6yozc7Kt8yGJRU0KFuarQCLcBGAs/s1600/arrow-down.png) no-repeat center transparent;
}
.thread-toggle.thread-expanded a {
    background-image: url(https://4.bp.blogspot.com/-iSlCbL2tuHc/WX-4kAA8s3I/AAAAAAAACzI/kDZT0aEUbaksawXUZmuxBzBtp2R4c3ZkwCLcBGAs/s1600/arrow-up.png);
}
.thread-toggle a:hover {
    opacity: 0.9;
}
.continue,
.loadmore,
.thread-chrome.thread-collapsed {display: none;}

/** @media (max-width: 414px) {
.avatar-image-container, .comment-replies .avatar-image-container {
    float: none;
    width: 70px;
    height: 70px;
}
.comment-block, .comment-replies .comment, .comment-replybox-single, .comment-replybox-thread,.comment-replies .comment-block {
    margin: 1rem 0 0;
}
}
**/

/**FIN CSS COMENTARIOS**/
 

<!-- CAMBIAR EL AÑO DEL COPYRIGHT -->
 
<script type="text/javascript">
copyright=new Date();
update=copyright.getFullYear();
document.write("© 2014 - " + update + " " + "Título de la web");
</script>

<!-- //CAMBIAR EL AÑO DEL COPYRIGHT --> 

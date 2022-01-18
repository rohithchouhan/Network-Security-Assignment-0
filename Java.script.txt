$( document ).ready(function() {

});
function enc(){
    var en =  document.getElementById("text1").value;
    var b='';
    for(let i=0;i<en.length;i++)
    {
      if(en.charCodeAt(i)<=122&&en.charCodeAt(i)>=97)
        b+=String.fromCharCode(122-((en.charCodeAt(i)-97)%26));
      else
      b+=en[i];
    }

    document.getElementById("screen1").innerHTML=b;
  }

  function dec(){
    var de =  document.getElementById("text2").value;
    var b='';
    for(let i=0;i<de.length;i++)
    {
      if(de.charCodeAt(i)<=122&&de.charCodeAt(i)>=97)
        b+=String.fromCharCode(122-((de.charCodeAt(i)-97)%26));
      else
        b+=de[i];
    }

    document.getElementById("screen2").innerHTML=b;
  }
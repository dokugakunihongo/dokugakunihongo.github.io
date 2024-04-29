---
layout: viewer
permalink: /view/
---

<iframe class="bg-light" src="" width="100%" height="900" allow="autoplay" id="drive"></iframe>
<script>
    document.addEventListener('DOMContentLoaded', function() {
        function obtenerParametro(nombre) {
            nombre = nombre.replace(/[\[]/, '\\[').replace(/[\]]/, '\\]');
            var regex = new RegExp('[\\?&]' + nombre + '=([^&#]*)');
            var resultados = regex.exec(location.search);
            return resultados === null ? '' : decodeURIComponent(resultados[1].replace(/\+/g, ' '));
        }
        var dato = obtenerParametro('dato');
        var drive = document.getElementById('drive');
        if(dato[2] == '/'){
            drive.src = "https://drive.google.com/file" + dato + "/preview";
        }else{
            drive.src = "https://drive.google.com/embeddedfolderview?id="+dato+"#list";
        }
    });
</script>

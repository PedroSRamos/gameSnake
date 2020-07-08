
<!DOCTYPE html>
<html>
    <head>
        <title>Game Snake</title>
    </head>
    <body>
        <div style="text-align: center;">
            <table border="0" width="100%">
            <tr>
            <td width=22%><div style="text-align: center;"><b>Instruções</b></div>
                <div style="text-align: center;">
                Com as setas do teclado mova a cobrinha comendo as maças e passe para a próxima fase atingindo a pontução!
                <p>Obs:Não colida com sigo mesmo pois perderá uma de suas vidas...</p>
                <p>Perdendo toda vida o jogo reiniciara! Caso queira reiniciar o jogo só clicar em "reinicïar jogo"!</p>
                </div>
                <form name="Frm1" method="post">
                    <div style="text-align: center;">
                     Nome : <input type="text" size="20" name="_nome">
                    </div>

                    <div style="text-align: center;">
                     fase : <input type="text" size="3" name="_fase" readonly value="1">
                    </div>
         
                    <div style="text-align: center;">
                     vidas : <input type="text" size="3" name="_vidas" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     pontução na fase: <input type="text" size="3" name="_total" readonly value="0">
                    </div>
        
                    <div style="text-align: center;">
                        pontução total: <input type="text" size="3" name="_total2" readonly value="0">
                    </div>
                    
                  </form>                
            </td>
            <td><canvas id="stage" width="600" height="600"></canvas></div></td>
            <td>
                <script>
                    document.write("<div style='text-align: center;'>Hanking:</div>");

                    if (localStorage["_nome1"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome1") + " - " + localStorage.getItem("_pontuacao1") + " pontos</div>");

                    if (localStorage["_nome2"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome2") + " - " + localStorage.getItem("_pontuacao2") + " pontos</div>");

                    if (localStorage["_nome3"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome3") + " - " + localStorage.getItem("_pontuacao3") + " pontos</div>");

                    if (localStorage["_nome4"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome4") + " - " + localStorage.getItem("_pontuacao4") + " pontos</div>");

                    if (localStorage["_nome5"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome5") + " - " + localStorage.getItem("_pontuacao5") + " pontos</div>");
                </script>
            </td>
            </tr>
            </table>
        </div>

        <script src="js/index.js" ></script>


         <div style="text-align: center;">
            <button onclick="reiniciar()" id="restarbtn" style="visibility: hidden; position: absolute;">
            </button>

            <button onclick="document.Frm1.action='game.html'; document.Frm1.submit();">
                Reiniciar jogo
            </button>
         </div>      

         <script>
            document.Frm1._nome.value = sessionStorage.getItem("_nome");
         </script>
    
    </body>

</html>

<!DOCTYPE html>
<html>
    <head>
        <title>Game Snake 2</title>
    </head>
    <body>
        <div style="text-align: center;">
            <table border="0" width="100%">
            <tr>
                <td width=20%><div style="text-align: center;"><b>Instruções</b></div>
                    <div style="text-align: center;">
                        Não se colida com a barra branca,perderá uma de suas vidas!
                    </div>
                <form name="Frm1" method="post">
                    <div style="text-align: center;">
                     Nome : <input type="text" size="20" name="_nome">
                    </div>

                    <div style="text-align: center;">
                     fase : <input type="text" size="3" name="_fase" readonly value="2">
                    </div>
         
                    <div style="text-align: center;">
                     vidas : <input type="text" size="3" name="_vidas" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     pontução na fase: <input type="text" size="3" name="_total" readonly value="0">
                    </div>
        
                    <div style="text-align: center;">
                        pontução total: <input type="text" size="3" name="_total2" readonly value="0">
                    </div>
                  </form>                
            </td>
            <td><canvas id="stage" width="600" height="600"></canvas></div></td>
            <td>
                <script>
                    document.write("<div style='text-align: center;'>Hanking:</div>");

                    if (localStorage["_nome1"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome1") + " - " + localStorage.getItem("_pontuacao1") + " pontos</div>");

                    if (localStorage["_nome2"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome2") + " - " + localStorage.getItem("_pontuacao2") + " pontos</div>");

                    if (localStorage["_nome3"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome3") + " - " + localStorage.getItem("_pontuacao3") + " pontos</div>");

                    if (localStorage["_nome4"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome4") + " - " + localStorage.getItem("_pontuacao4") + " pontos</div>");

                    if (localStorage["_nome5"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome5") + " - " + localStorage.getItem("_pontuacao5") + " pontos</div>");
                </script>
            </td>
            </tr>
            </table>
        </div>

        <script src="js/index_2.js" ></script>


         <div style="text-align: center;">
            <button onclick="reiniciar()" id="restarbtn" style="visibility: hidden; position: absolute;">
            </button>

            <button onclick="document.Frm1.action='game.html'; document.Frm1.submit();">
                Reiniciar jogo
            </button>
         </div>      

         <script>
            document.Frm1._nome.value = sessionStorage.getItem("_nome");
            document.Frm1._vidas.value = sessionStorage.getItem("_vidas");
            document.Frm1._total2.value = sessionStorage.getItem("_total2");
         </script>
    </body>

</html>

<!DOCTYPE html>
<html>
    <head>
        <title>Game Snake</title>
    </head>
    <body>
        <div style="text-align: center;">
            <table border="0" width="100%">
            <tr>
                <td width=20%><div style="text-align: center;"><b>Instruções</b></div>
                    <div style="text-align: center;">
                        Não se colida com a barra branca,perderá uma de suas vidas!
                    </div>
                <form name="Frm1" method="post">
                    <div style="text-align: center;">
                     Nome : <input type="text" size="20" name="_nome">
                    </div>

                    <div style="text-align: center;">
                     fase : <input type="text" size="3" name="_fase" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     vidas : <input type="text" size="3" name="_vidas" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     pontução na fase: <input type="text" size="3" name="_total" readonly value="0">
                    </div>
        
                    <div style="text-align: center;">
                        pontução total: <input type="text" size="3" name="_total2" readonly value="0">
                    </div>
                  </form>                
            </td>
            <td><canvas id="stage" width="600" height="600"></canvas></div></td>
            <td>
                <script>
                    document.write("<div style='text-align: center;'>Hanking:</div>");

                    if (localStorage["_nome1"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome1") + " - " + localStorage.getItem("_pontuacao1") + " pontos</div>");

                    if (localStorage["_nome2"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome2") + " - " + localStorage.getItem("_pontuacao2") + " pontos</div>");

                    if (localStorage["_nome3"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome3") + " - " + localStorage.getItem("_pontuacao3") + " pontos</div>");

                    if (localStorage["_nome4"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome4") + " - " + localStorage.getItem("_pontuacao4") + " pontos</div>");

                    if (localStorage["_nome5"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome5") + " - " + localStorage.getItem("_pontuacao5") + " pontos</div>");
                </script>
            </td>
            </tr>
            </table>
        </div>

        <script src="js/index_3.js" ></script>


         <div style="text-align: center;">
            <button onclick="reiniciar()" id="restarbtn" style="visibility: hidden; position: absolute;">
            </button>

            <button onclick="document.Frm1.action='game.html'; document.Frm1.submit();">
                Reiniciar jogo
            </button>
         </div>      

         <script>
            document.Frm1._nome.value = sessionStorage.getItem("_nome");
            document.Frm1._vidas.value = sessionStorage.getItem("_vidas");
            document.Frm1._total2.value = sessionStorage.getItem("_total2");
         </script>         
    </body>

</html>

<!DOCTYPE html>
<html>
    <head>
        <title>Game Snake</title>
    </head>
    <body>
        <div style="text-align: center;">
            <table border="0" width="100%">
            <tr>
                <td width=20%><div style="text-align: center;"><b>Instruções</b></div>
                    <div style="text-align: center;">
                        Não se colida com a barra branca,perderá uma de suas vidas!
                    </div>
                <form name="Frm1" method="post">
                    <div style="text-align: center;">
                     Nome : <input type="text" size="20" name="_nome">
                    </div>

                    <div style="text-align: center;">
                     fase : <input type="text" size="3" name="_fase" readonly value="4">
                    </div>
         
                    <div style="text-align: center;">
                     vidas : <input type="text" size="3" name="_vidas" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     pontução na fase: <input type="text" size="3" name="_total" readonly value="0">
                    </div>
        
                    <div style="text-align: center;">
                        pontução total: <input type="text" size="3" name="_total2" readonly value="0">
                    </div>
                  </form>                
            </td>
            <td><canvas id="stage" width="600" height="600"></canvas></div></td>
            <td>
                <script>
                    document.write("<div style='text-align: center;'>Hanking:</div>");

                    if (localStorage["_nome1"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome1") + " - " + localStorage.getItem("_pontuacao1") + " pontos</div>");

                    if (localStorage["_nome2"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome2") + " - " + localStorage.getItem("_pontuacao2") + " pontos</div>");

                    if (localStorage["_nome3"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome3") + " - " + localStorage.getItem("_pontuacao3") + " pontos</div>");

                    if (localStorage["_nome4"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome4") + " - " + localStorage.getItem("_pontuacao4") + " pontos</div>");

                    if (localStorage["_nome5"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome5") + " - " + localStorage.getItem("_pontuacao5") + " pontos</div>");
                </script>
            </td>
            </tr>
            </table>
        </div>

        <script src="js/index_4.js" ></script>


         <div style="text-align: center;">
            <button onclick="reiniciar()" id="restarbtn" style="visibility: hidden; position: absolute;">
            </button>

            <button onclick="document.Frm1.action='game.html'; document.Frm1.submit();">
                Reiniciar jogo
            </button>
         </div>      

         <script>
            document.Frm1._nome.value = sessionStorage.getItem("_nome");
            document.Frm1._vidas.value = sessionStorage.getItem("_vidas");
            document.Frm1._total2.value = sessionStorage.getItem("_total2");
         </script>         
    </body>

</html>

<!DOCTYPE html>
<html>
    <head>
        <title>Game Snake</title>
    </head>
    <body>
        <div style="text-align: center;">
            <table border="0" width="100%">
            <tr>
                <td width=20%><div style="text-align: center;"><b>Instruções</b></div>
                    <div style="text-align: center;">
                        Não se colida com a barra branca,perderá uma de suas vidas!
                    </div>
                <form name="Frm1" method="post">
                    <div style="text-align: center;">
                     Nome : <input type="text" size="20" name="_nome">
                    </div>

                    <div style="text-align: center;">
                     fase : <input type="text" size="3" name="_fase" readonly value="5">
                    </div>
         
                    <div style="text-align: center;">
                     vidas : <input type="text" size="3" name="_vidas" readonly value="3">
                    </div>
         
                    <div style="text-align: center;">
                     pontução na fase: <input type="text" size="3" name="_total" readonly value="0">
                    </div>
        
                    <div style="text-align: center;">
                        pontução total: <input type="text" size="3" name="_total2" readonly value="0">
                    </div>
                  </form>                
            </td>
            <td><canvas id="stage" width="600" height="600"></canvas></div></td>
            <td>
                <script>
                    document.write("<div style='text-align: center;'>Hanking:</div>");

                    if (localStorage["_nome1"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome1") + " - " + localStorage.getItem("_pontuacao1") + " pontos</div>");

                    if (localStorage["_nome2"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome2") + " - " + localStorage.getItem("_pontuacao2") + " pontos</div>");

                    if (localStorage["_nome3"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome3") + " - " + localStorage.getItem("_pontuacao3") + " pontos</div>");

                    if (localStorage["_nome4"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome4") + " - " + localStorage.getItem("_pontuacao4") + " pontos</div>");

                    if (localStorage["_nome5"])
                      document.write("<div style='text-align: center;'>" + localStorage.getItem("_nome5") + " - " + localStorage.getItem("_pontuacao5") + " pontos</div>");
                </script>
            </td>
            </tr>
            </table>
        </div>

        <script src="js/index_5.js" ></script>


         <div style="text-align: center;">
            <button onclick="reiniciar()" id="restarbtn" style="visibility: hidden; position: absolute;">
            </button>

            <button onclick="document.Frm1.action='game.html'; document.Frm1.submit();">
                Reiniciar jogo
            </button>
         </div>          

         <script>
            document.Frm1._nome.value = sessionStorage.getItem("_nome");
            document.Frm1._vidas.value = sessionStorage.getItem("_vidas");
            document.Frm1._total2.value = sessionStorage.getItem("_total2");
         </script>         
    </body>

</html>

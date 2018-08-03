<%@ Master Language="C#" AutoEventWireup="true" CodeFile="Site.master.cs" Inherits="SiteMaster" %>
 
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en">
<head runat="server">
    <title></title>

    <%--<meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">--%>


    <asp:ContentPlaceHolder ID="HeadContent" runat="server">
    </asp:ContentPlaceHolder>



<!-- Estilos -->
<%--<meta content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" name="viewport">--%>
<!-- Bootstrap 3.3.7 -->
<link rel="stylesheet" href="~/Styles/2018/css/bootstrap.min.css">
<!-- Font Awesome -->
<link rel="stylesheet" href="~/Styles/2018/css/font-awesome.min.css">

<!-- Theme style -->
<link rel="stylesheet" href="~/Styles/2018/css/principal.css">
<link rel="stylesheet" href="~/Styles/2018/css/skins.css">
 

<!-- Elegir rango de Fecha -->
<link rel="stylesheet" href="~/Styles/2018/css/bootstrap-datepicker.min.css">



<!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
<!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
<!--[if lt IE 9]>
<script src="https://oss.maxcdn.com/html5shiv/3.7.3/html5shiv.min.js"></script>
<script src="https://oss.maxcdn.com/respond/1.4.2/respond.min.js"></script>
<![endif]-->



<!-- jQuery 3 -->
<script src="Styles/2018/js/jquery.min.js"></script>
<!-- Bootstrap 3.3.7 -->
<script src="Styles/2018/js/bootstrap.min.js"></script>
<script src="Styles/2018/js/adminlte.min.js"></script>








<%--    <!-- Estilos -->
    <link href='https://fonts.googleapis.com/css?family=Pontano+Sans' rel='stylesheet' type='text/css'>
    <!-- Bootstrap -->
    <link href='~/Styles/2015/css/bootstrap.css' rel="stylesheet">
    <!-- Iconos / javascript plugins -->
    <link href='~/Styles/2015/css/plugins.css' rel="stylesheet">
    <!-- Estilos Base -->
    <link href='~/Styles/2015/css/principal.css' rel="stylesheet">
    <!-- Colores / elementos -->
    <link href='~/Styles/2015/css/colores.css' rel="stylesheet">

    <link href='~/Styles/2015/css/mensajes/jquery.toastmessage-min.css' rel="stylesheet" type="text/css">--%>


    <!-- Menu movil -->
    <%--<link rel="stylesheet" type="text/css" href="~/Styles/2015/menu/css/component.css" />
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/2015/menu/js/modernizr.custom.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
--%>

<%--<script type="text/javascript">
        document.oncontextmenu = function () { return false; }
</script>--%>

</head>


<body class="hold-transition skin-blue sidebar-mini">
    <form runat="server">

    <!-- Modernizr -->
    <script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/2015/js/vendor/modernizr-2.6.2-respond-1.1.0.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>


    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery-1.11.3.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery-ui-1.10.3.custom.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.blockUI.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.alerts.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/alertify.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.bpopup.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.quicksearch.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.numeric.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/MasterPage.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/Services.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/EventTesting.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/2015/css/mensajes/jquery.toastmessage-min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript">

        SetBaseUrl('<%= Page.ResolveClientUrl("~/") %>');
        SetWebPagePath('<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"] %>');
        SetWebVersion('<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>');

    </script>

    <%--<asp:ToolkitScriptManager ID="ToolkitScriptManager1" runat="server" CombineScripts="True" EnableScriptGlobalization="True" AsyncPostBackTimeout="120000" ScriptMode="Release" />--%>
    <asp:ScriptManager ID="ToolkitScriptManager1" runat="server" EnableScriptGlobalization="True" AsyncPostBackTimeout="120000" ScriptMode="Release" />


  
<!-- /Total -->
<div id="st-container" class="st-container">

<!-- Contenedor principal -->
<div id="contenedor_de_pagina" class="ancho_de_pagina" >






    <!-- Cabecera-->
    <header class="menu menu-estilo1">
 
    <div class="menu-interior" style="height: 54px!important;">
    <!-- div#fila-ajustable -->
    <div class="fila-ajustable">




    <header class="main-header">
    
    <div class="">
    <!-- Ocultar Menu -->
    <a href="#" class="bajar_movil alinear_icono_menu" data-toggle="push-menu" role="button" >
        <asp:Image ID="Image11" runat="server" ImageUrl="~/Styles/img/icono_menu.jpg" class="icono_menu" />
    </a>
    </header>




            <asp:UpdatePanel ID="upShoppingCar" runat="server" ClientIDMode="Static">
            <ContentTemplate>
        

        <!-- Menu tablet -->
        <%--<div id="st-trigger-effects" class="">
			<button id="Button1" runat="server" data-effect="st-effect-1" style="background:#ffffff; border:1px solid #ffffff;padding: 12px;">
             <asp:Image ID="Image2" runat="server" 
                    ImageUrl="~/Styles/2015/img/icono_menu4.png" Width="26px" />
            </button>
		</div>--%>

        <div class=" ocultar_en_celular ocultar_en_tablet ocultar_en_pc">
            <ul class="menu colocar_izquierda">
                <!-- Icono en Pc -->
                <li style="display:none">
                <%--<li class="visible_en_pc">--%>
                    <a href="#" id="desplazar_menu_izquierda" >
                        <i class="icono_desplazar_menu_izquierda" ></i>
                    </a>
                </li>


                <!-- /Icono en Pc -->

                <!-- Icono en Tablet -->
                <li style="display:none">
                <%--<li class="visible_en_tablet">--%>
                    <a href="#" data-toggle="collapse" data-target=".menu_desplegable" >
                        <i class="icono_desplazar_menu_izquierda"></i>
                    </a>
                </li>
                <!-- /Icono en Tablet -->

            </ul>
        </div>
        <!-- /Menu tablet -->



        <!-- Logo -->
        <div class="">
            <div id="contenedor_logo_principal">
            <asp:Image ID="imgLogoGanoLife" runat="server" 
                    ImageUrl="~/Styles/2015/img/logo.png" CssClass="colocar_izquierda bajar_logo logo_movil" 
                    AlternateText="Logo GanoLife" ToolTip="Logo GanoLife" 
                    meta:resourcekey="imgLogoGanoLifeResource1"/>
            <asp:Image ID="imgline" runat="server" 
                    ImageUrl="~/Styles/2015/img/linea_de_division.png" CssClass="colocar_izquierda" 
                    ToolTip="Logo GanoLife" meta:resourcekey="imglineResource1"/>

            <div class="colocar_busqueda_principal " TabIndex="1" >
            <asp:TextBox ID="txtSearchSuggestion" runat="server" ClientIDMode="Static" 
                    CssClass="campo_texto_busqueda_principal colocar_izquierda" MaxLength="30" 
            placeholder="Que desea hacer hoy" meta:resourcekey="txtSearchResource1"></asp:TextBox>
            </div>


<%--            <div class="colocar_derecha colocar_webkit" style="margin-top: 10px;">
            <table width="80px" border="0" align="left" cellpadding="8" cellspacing="8" style="margin-top:-6px; margin-left:20px;">
                  <tr>
                    <td align="left">
                    <asp:ImageButton ID="btnEnglish" runat="server" CommandArgument="en-US" OnClientClick='ChangeLanguage("en-US");' ToolTip="Ingles" ImageUrl="~/Styles/2015/img/banderas1.gif" 
                        meta:resourcekey="btnEnglishResource1" />
                    </td>

                    <td align="right">
                    
                    <asp:ImageButton ID="btnSpanish" runat="server" CommandArgument="es-PE" OnClientClick='ChangeLanguage("es-PE");' ToolTip="Español" ImageUrl="~/Styles/2015/img/banderas3.gif"
                        meta:resourcekey="btnSpanishResource1" />
                       
                    </td>
                    boton_paises
                  </tr>
                </table>
            </div>--%>


             <!-- Idiomas -->
             <ul class="colocar_derecha colocar_botones_principal" style="margin-top: 10px;" >
                    <li class="desplegable notificaciones_desplegable">
                        <asp:HyperLink ID="lnkCurrentLanguage" runat="server" NavigateUrl="#" TabIndex="5" 
                        class="boton_basico boton_idiomas" data-toggle="desplegable" >
                            <asp:Image ID="imgCurrentLanguage" runat="server" CssClass="icono_adaptable_pais_s" meta:resourcekey="imgCurrentLanguageResource1"/>
&nbsp;&nbsp;
                        </asp:HyperLink>
                            <ul class="menu_desplegable menu_desplegable_alinear_idiomas aparecer3" style="z-index: 1100; box-shadow: 0 3px 15px rgba(0,0,0,.5) !important;">

                                 <asp:DataList ID="dtlLanguage" runat="server" RepeatColumns="3" ClientIDMode="Static"
                                    RepeatDirection="Horizontal" onitemdatabound="dtlLanguage_ItemDataBound" 
                                     meta:resourcekey="dtlLanguageResource1" >
                                <ItemTemplate>
                                    <div class="etiqueta menu_desplegable_item" align="center" style="margin-top: 10px;">
                                        <asp:HiddenField ID="hdCode" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "Code") %>' />
                                        <div class="itemborde efecto_zoom" align="center">
                                        <asp:ImageButton ID="imgSelectLanguage" runat="server" 
                                                CssClass="icono_adaptable_pais" OnClientClick='<%# "ChangeLanguage(\""+DataBinder.Eval(Container.DataItem, "Code")+"\");" %>'
                                                OnClick="imgSelectLanguage_Click" />
                                        </div>
                                        <br>
                                        <asp:Label ID="lbSelectLanguage" runat="server" 
                                            Text='<%# DataBinder.Eval(Container.DataItem, "Description") %>' 
                                            CssClass="texto_gris" Font-Bold="False" ></asp:Label>

                                    </div>
                                </ItemTemplate>
                            </asp:DataList>

                            </ul>
                    </li>  
             </ul>


            <!-- Empresas -->
            <ul class="colocar_derecha colocar_botones_principal" style="margin-top: 10px;" >
                    <li class="desplegable notificaciones_desplegable">
                        <asp:LinkButton ID="lnkCurrentCompany" runat="server" href="#" TabIndex="4"
                            class="boton_basico boton_empresas" data-toggle="desplegable" >
                            <asp:Image ID="imgCurrentCompany" runat="server" CssClass="icono_adaptable_empresa_s"  meta:resourcekey="imgCurrentCompanyResource1"/>
&nbsp;&nbsp;
                            <asp:Label ID="lbCurrentCompany" runat="server" Text="Empresas" 
                            CssClass="ocultar_en_tablet_landscape boton_empresas_alinear_texto" 
                            meta:resourcekey="lbCurrentCompanyResource1" ></asp:Label>
</asp:LinkButton>

                            <ul class="menu_desplegable menu_desplegable_alinear_empresas aparecer3" style="z-index: 1100; box-shadow: 0 3px 15px rgba(0,0,0,.5) !important;">

                            <asp:DataList ID="dtlCompanyAccess" runat="server" RepeatColumns="3" ClientIDMode="Static"
                            RepeatDirection="Horizontal" onitemdatabound="dtlCompanyAccess_ItemDataBound" meta:resourcekey="dtlCompanyAccessResource1" >
                                     <ItemTemplate>
                                         <div align="center" class="etiqueta menu_desplegable_item" 
                                             style="margin-top: 10px;">
                                             <asp:HiddenField ID="hdCompanyID" runat="server" 
                                                 Value='<%# DataBinder.Eval(Container.DataItem, "CompanyID") %>' />
                                             <div align="center" class="itemborde efecto_zoom">
                                                 <asp:ImageButton ID="imgSelectCompany" runat="server" 
                                                     CssClass="icono_adaptable_empresas" 
                                                     meta:resourcekey="imgSelectCompanyResource1" OnClick="imgSelectCompany_Click" />
                                             </div>
                                             <br>
                                             <asp:Label ID="lbSelectCompany" runat="server" CssClass="texto_gris" 
                                                 Font-Bold="False" meta:resourcekey="lbSelectCompanyResource1" 
                                                 Text='<%# DataBinder.Eval(Container.DataItem, "CompanyName") %>'></asp:Label>
                                             </br>
                                         </div>
                                     </ItemTemplate>
                            </asp:DataList>

                            </ul>
                    </li>
             </ul>


            <!-- Paises -->
            <ul class="colocar_derecha colocar_botones_principal" style="margin-top: 10px;" >
                    <li class="desplegable notificaciones_desplegable">
                        <asp:LinkButton ID="lnkCurrentCountry" runat="server" href="#" TabIndex="3" 
                        class="boton_basico boton_paises" data-toggle="desplegable" >
                            <asp:Image ID="imgCurrentCountry" runat="server" CssClass="icono_adaptable_pais_s"  meta:resourcekey="imgCurrentCountryResource1"/>
&nbsp;&nbsp;
                        <asp:Label ID="lbCurrentCountry" runat="server" Text="Paises" 
                            CssClass="ocultar_en_tablet_landscape boton_paises_alinear_texto" 
                            meta:resourcekey="lbCurrentCountryResource1"></asp:Label>
</asp:LinkButton>

                            <ul class="menu_desplegable menu_desplegable_alinear_paises aparecer3" style="z-index: 1100; box-shadow: 0 3px 15px rgba(0,0,0,.5) !important;">

                            <asp:DataList ID="dtlCountryAccess" runat="server" RepeatColumns="3" ClientIDMode="Static"
                            RepeatDirection="Horizontal" onitemdatabound="dtlCountryAccess_ItemDataBound" meta:resourcekey="dtlCountryAccessResource1" >
                                    <ItemTemplate>
                                    <div class="etiqueta menu_desplegable_item" align="center" style="margin-top: 10px;">
                                        <asp:HiddenField ID="hdCountryID" runat="server" 
                                            Value='<%# DataBinder.Eval(Container.DataItem, "CountryID") %>' />
                                        <div class="itemborde efecto_zoom" align="center">
                                        <asp:ImageButton ID="imgSelectCountry" runat="server" 
                                                CssClass="icono_adaptable_pais" onclick="imgSelectCountry_Click" 
                                                meta:resourcekey="imgSelectCountryResource1" />
                                        </div>
                                        <br>
                                        <asp:Label ID="lbSelectCountry" runat="server" 
                                            Text='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' 
                                            CssClass="texto_gris" Font-Bold="False" 
                                            meta:resourcekey="lbSelectCountryResource1" ></asp:Label>

                                    </div>
                                </ItemTemplate>
                            </asp:DataList>

                            </ul>
                    </li>
             </ul>


            <!-- Favoritos -->
             <ul class="colocar_derecha colocar_botones_principal" style="margin-top: 10px;" >
                    <li class="desplegable notificaciones_desplegable">
                        <asp:HyperLink ID="lnkFav" runat="server" NavigateUrl="#" TabIndex="2" 
                            class="boton_basico boton_favoritos" data-toggle="desplegable">
                            <asp:Label ID="lblFav1" runat="server" Text="Favoritos" meta:resourcekey="lblFav1Resource1" ></asp:Label>
</asp:HyperLink>         
                            <ul class="menu_desplegable menu_desplegable_alinear_favoritos aparecer3" style="z-index: 1100; box-shadow: 0 3px 15px rgba(0,0,0,.5) !important;">
                                <table width="380px" border="0" align="center" cellpadding="10" cellspacing="0" >
                                <tr>
                                <td width="25%" align="center">
                                <asp:HyperLink ID="lnkFavIcon1" runat="server" NavigateUrl="~/Dashboard.aspx#top"  ><asp:Image ID="imgFavIcon1" 
                                        runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" ImageUrl="~/Styles/2015/img/icono_fav_1.png" />
<br>
                                <asp:Label ID="lblTextFav1" runat="server" Text="Dashboard" CssClass="texto_gris" 
                                        meta:resourcekey="lblTextFav1Resource1" ></asp:Label>
</asp:HyperLink>
                                <br><br>
                                </td>

                                <td width="25%" align="center" >
                                <asp:HyperLink ID="lnkFavIcon2" runat="server" 
                                NavigateUrl="~/Reports/Management/ManagementDashboard.aspx#top" >
                                <asp:Image ID="imgFavIcon2" runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" 
                                        ImageUrl="~/Styles/2015/img/icono_fav_6.png"  />
<br>
                                <asp:Label ID="lblTextFav2" runat="server" Text="Reportes Gerenciales" 
                                        CssClass="texto_gris" meta:resourcekey="lblTextFav2Resource1"></asp:Label>
</asp:HyperLink>
                                </td>

                                <td width="25%" align="center">
                                <asp:HyperLink ID="lnkFavIcon3" runat="server" 
                                        NavigateUrl="~/Modules/CRM/CRMNewCustomer.aspx" ><asp:Image ID="imgFavIcon3" 
                                        runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" 
                                        ImageUrl="~/Styles/2015/img/icono_fav_3.png"  />
<br>
                                <asp:Label ID="lblTextFav3" runat="server" Text="Nueva Afiliación" CssClass="texto_gris" 
                                        meta:resourcekey="lblTextFav3Resource1"></asp:Label>
</asp:HyperLink>
                                
                                </td>

                                <td width="25%" align="center">
                                <asp:HyperLink ID="lnkFavIcon4" runat="server" 
                                        NavigateUrl="~/Modules/Orders/NewOrder.aspx#top" ><asp:Image ID="imgFavIcon4" 
                                        runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" 
                                        ImageUrl="~/Styles/2015/img/icono_fav_5.png" />
<br>
                                <asp:Label ID="lblTextFav4" runat="server" Text="Nuevo Pedido" 
                                        CssClass="texto_gris" meta:resourcekey="lblTextFav4Resource1"></asp:Label>
</asp:HyperLink>

                                </td>

                                </tr>



                                <tr>

                                <td width="25%" align="center">
                                    <asp:HyperLink ID="lnkFavIcon6" runat="server" NavigateUrl="~/Modules/WarehouseManager/ShippingOrder.aspx#top" >
                                    <asp:Image ID="imgFavIcon6" runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" ImageUrl="~/Styles/2015/img/icono_fav_11.png" />
                                    <br>
                                    <asp:Label ID="lblTextFav6" runat="server" Text="Entrega de Pedido" CssClass="texto_gris" meta:resourcekey="lblTextFav6Resource1"></asp:Label>
                                    </asp:HyperLink>
                                </td>

                                <td width="25%" align="center">
                                    <asp:HyperLink ID="lnkFavIcon5" runat="server" NavigateUrl="http://ganolife.pe/Correo/" Target="_blanck"  >
                                    <asp:Image ID="imgFavIcon5" runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" ImageUrl="~/Styles/2015/img/icono_fav_8.png" />
                                    <br>
                                    <asp:Label ID="lblTextFav5" runat="server" Text="Email" CssClass="texto_gris" meta:resourcekey="lblTextFav5Resource1"></asp:Label>
                                    </asp:HyperLink>
                                </td>

                                <td width="25%" align="center" >
                                    <asp:HyperLink ID="HyperLink5" runat="server" NavigateUrl="~/Modules/CRM/Genealogy.aspx#top" >
                                    <asp:Image ID="Image1" runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" ImageUrl="~/Styles/2015/img/icono_fav_2.png" />
                                    <br>
                                    <asp:Label ID="Label23" runat="server" Text="Genealogía" CssClass="texto_gris" meta:resourcekey="Label23Resource1"></asp:Label>
                                    </asp:HyperLink>
                                </td>

                                <td width="25%" align="center" >
                                    <asp:HyperLink ID="HyperLink7" runat="server" NavigateUrl="~/Modules/Reports/Dashboard.aspx" >
                                    <asp:Image ID="Image4" runat="server" CssClass="efecto_zoom icono_adaptable_favoritos" ImageUrl="~/Styles/2015/img/icono_fav_7.png" />
                                    <br>
                                    <asp:Label ID="Label25" runat="server" Text="Reportes" CssClass="texto_gris" meta:resourcekey="Label25Resource1"></asp:Label>
                                    </asp:HyperLink>
                                </td>

                                </tr>
                                </table>
                            </ul>
                    </li>  
             </ul>
          
    
            </div>    
        </div>
        <!-- /Logo -->


        <!-- Navegacion derecha -->
        <div id="cabecera_seccion_menu" >
        
            <asp:LoginView ID="HeadLoginView" runat="server" EnableViewState="False">

                <AnonymousTemplate>
                <a href="~/Login.aspx" ID="HeadLoginStatus" runat="server" style="text-decoration: none" >
                <asp:Label ID="lblLogin" runat="server" Text="LOGIN" Font-Names="Arial" ForeColor="White" meta:resourcekey="lblLoginResource1"></asp:Label>
                        &nbsp;&nbsp;
                </a>
                </AnonymousTemplate>


                <LoggedInTemplate>
                <!-- Usuario -->
                <div class="colocar_derecha arriba">
                <table  width="700" border="0" align="right" cellpadding="0" cellspacing="0">
                  <tr>
                    <td width="572">
                    <div class="menu colocar_derecha subir_salir">
                    <asp:LoginName ID="HeadLoginName" runat="server" CssClass="texto_en_tablet ocultar_en_tablet2" ForeColor="#27C266" 
                            meta:resourcekey="HeadLoginNameResource1"/> 
                    <asp:Label ID="lblLoginUserID" runat="server" CssClass="texto_en_tablet" 
                            meta:resourcekey="lblLoginUserIDResource1"></asp:Label>
                    </div>
                    </td>

                    <td width="72">
                    <div class="menu colocar_derecha subir_salir">
                    <asp:LoginStatus ID="HeadLoginStatus" runat="server" LogoutAction="Redirect" CssClass="texto_en_tablet2" 
                    LogoutText="Salir" LogoutPageUrl="~/" TabIndex="6" meta:resourcekey="HeadLoginStatusResource1" />
                    </div>
                    </td>

                    <td width="72">
                    </td>
                  </tr>
                </table>
                </div>
                <!-- /Usuario -->
                </LoggedInTemplate>

            </asp:LoginView>

            <!-- Menu Tablet, se muestra solo en esa resolucion -->
            <ul class="menu colocar_izquierda visible_en_celular2222">
                <li><a href="#" data-toggle="collapse" data-target=".menu_desplegable"><i class="icono_desplazar_menu_izquierda"></i></a></li>
                <li class="linea_division_vertical"></li>
            </ul>
            <!-- /Menu Tablet -->

        </div>
        <!-- /Navegacion derecha -->



            </ContentTemplate>
            </asp:UpdatePanel>



    </div>
    <!-- /div#fila-ajustable -->
    </div>

    </header>
    <!-- /Cabecera-->




<!--Nuevo Menu Principal -->
<aside class="main-sidebar">
    <section class="sidebar">
      <ul class="sidebar-menu" data-widget="tree">
       
        <li>
          <asp:LinkButton ID="LinkButton2" runat="server" href="Dashboard.aspx" class="icono_inicio" >
            <i class="fa"></i>
            <asp:Label ID="Label37" runat="server" Text="Inicio" class="texto_menu" ></asp:Label>  
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton3" runat="server" href="#" class="icono_zarpe" >
            <i class="fa"></i>
            <asp:Label ID="Label6" runat="server" Text="Zarpe" class="texto_menu" ></asp:Label>  
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton4" runat="server" href="Modules/Genealogy/Genealogy.aspx" class="icono_genealogia" >
            <i class="fa"></i>
            <asp:Label ID="Label12" runat="server" Text="Genealogía" class="texto_menu" ></asp:Label>  
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton6" runat="server" href="Modules/Commissions/HistoricoCiclo.aspx" class="icono_comisiones" >
            <i class="fa"></i>
            <asp:Label ID="Label115" runat="server" Text="Comisiones" class="texto_menu" ></asp:Label> 
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton7" runat="server" href="Modules/Compras/HistoricoCompras.aspx" class="icono_compras" >
            <i class="fa"></i>
            <asp:Label ID="Label116" runat="server" Text="Mis compras" class="texto_menu" ></asp:Label> 
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton8" runat="server" href="Modules/Inscribir/Inscribir_1.aspx" class="icono_inscribir" >
            <i class="fa"></i>
            <asp:Label ID="Label117" runat="server" Text="Inscribir" class="texto_menu" ></asp:Label>
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton9" runat="server" href="Modules/Creditos/ComprarConCreditos.aspx" class="icono_creditos" >
            <i class="fa"></i>
            <asp:Label ID="Label118" runat="server" Text="Créditos" class="texto_menu" ></asp:Label>
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton10" runat="server" href="Modules/Suscripcion/NoInscrito.aspx" class="icono_suscripcion" >
            <i class="fa"></i>
            <div style="margin-top:-25px; line-height: 1; " class="mover_izquierda_1">
            <asp:Label ID="Label119" runat="server" Text="Suscripción " class="texto_menu" ></asp:Label> <br> 
            <asp:Label ID="Label111" runat="server" Text="Mensual" class="texto_menu" ></asp:Label>  
            </div>     
            <%--<asp:Label ID="Label19" runat="server" Text="SuscripciónMensual" class="texto_menu" ></asp:Label> --%>   
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton11" runat="server" href="Modules/X5/X5.aspx" class="icono_x5" >
            <i class="fa"></i>
            <asp:Label ID="Label20" runat="server" Text="Mi equipo X5" class="texto_menu" ></asp:Label>
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton12" runat="server" href="Modules/X3/X3.aspx" class="icono_x3" >
            <i class="fa"></i>
            <asp:Label ID="Label18" runat="server" Text="Mi equipo X3" class="texto_menu" ></asp:Label>    
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton13" runat="server" href="Modules/Extralife/Extralife.aspx" class="icono_extralife" >
            <i class="fa"></i>
            <asp:Image ID="Image6" runat="server" ImageUrl="~/Styles/img/icono_menu_extralife_texto.png" 
            style="margin-top:-14px;" class="extralife_texto"/>
            <asp:Image ID="Image7" runat="server" ImageUrl="~/Styles/img/icono_menu_extralife_texto_on.png" 
            style="margin-top:-14px;" class="extralife_texto_on"/>
            <%--<asp:Label ID="Label22" runat="server" Text="Extralife" class="texto_menu" ></asp:Label> --%>       
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton14" runat="server" href="Modules/Herramientas/Descarga.aspx" class="icono_herramientas" >
            <i class="fa"></i>
            <asp:Label ID="Label19" runat="server" Text="Herramientas" class="texto_menu" ></asp:Label>    
          </asp:LinkButton>
        </li>

        <li>
          <asp:LinkButton ID="LinkButton15" runat="server" href="Modules/Contacto/Contacto.aspx" class="icono_ayuda" >
            <i class="fa"></i>
            <asp:Label ID="Label24" runat="server" Text="¿Quieres ayuda?" class="texto_menu" ></asp:Label>    
          </asp:LinkButton>
        </li>
  
        <li>
          <div class="" style="border:1px solid #cccccc; padding:5px; margin:12px 11px 3px 20px ; ">
            <asp:Image ID="Image15" runat="server" ImageUrl="~/Styles/img/icono_telefono.png"/>
            <asp:Label ID="Label39" runat="server" Text="¡Contáctanos!" ForeColor="#8e8e8e" class="texto_home_13" ></asp:Label>         
          </div>
        </li>

      </ul>
    </section>
</aside>









    <asp:UpdatePanel ID="upMenu" runat="server" ClientIDMode="Static">
    <ContentTemplate>




<!-- Contenido total lado izquierda -->
<table border="0" align="center" cellpadding="8" cellspacing="8" style="width:94%!important;  ">
            <tr>
            <td align="left">


            <!-- Menu Principal -->
            <div  class="ocultar_en_pc"  runat="server" style="height: 90px!important;">
            <div id="menu_inicio">
                        <asp:HyperLink ID="lnkHome" runat="server" NavigateUrl="~/Dashboard.aspx#top" TabIndex="7"
                        CssClass="menu_inicio_borde icono_menu icono_inicio ancho_item_menu" >
                        <i class="icono_espacio_menu"></i><asp:Label ID="lblMenuHome" runat="server" Text="Dashboard" meta:resourcekey="lblMenuHomeResource1" ></asp:Label>
                        </asp:HyperLink>
            </div>
            <div id="menu_crm">
                        <%--<asp:HyperLink ID="HyperLink1" runat="server" CssClass="menu_crm_borde" >--%>
                        <asp:HyperLink ID="lnkCRM" runat="server" NavigateUrl="~/Modules/CRM/CRMdashboard.aspx#top" TabIndex="8" 
                        CssClass="menu_inicio_borde icono_menu icono_cmr ancho_item_menu" >
                        <i class="icono_espacio_menu"></i><asp:Label ID="Label1" runat="server" Text="CRM" meta:resourcekey="Label1Resource1" ></asp:Label>
                        </asp:HyperLink>  
            </div>
            <div id="menu_ventas">
                        <%--<asp:HyperLink ID="HyperLink2" runat="server" CssClass="menu_ventas_borde" >--%>
                        <asp:HyperLink ID="lnkSales" runat="server" NavigateUrl="~/Modules/Orders/OrderDashboard.aspx#top" TabIndex="9" 
                        CssClass="menu_inicio_borde icono_menu icono_distribuidores ancho_item_menu" ><i class="icono_espacio_menu"></i> <asp:Label 
                        ID="Label5" runat="server" Text="Pedidos" meta:resourcekey="Label5Resource1" ></asp:Label>
                        </asp:HyperLink>
            </div>
            <div id="menu_sucursales">
                        <%--<asp:HyperLink ID="HyperLink2" runat="server" CssClass="menu_sucursales_borde" >--%>
                        <asp:HyperLink ID="lnkBranchOffice" runat="server" NavigateUrl="~/Modules/WarehouseManager/Home.aspx#top" TabIndex="10" 
                            CssClass="menu_inicio_borde icono_menu icono_pedidos ancho_item_menu" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="lblBranchManagement" runat="server" Text="Entrega de Mercadería" meta:resourcekey="lblBranchManagementResource1"></asp:Label>
                        </asp:HyperLink>
            </div>
            <div id="menu_reportes">
                        <%--<asp:HyperLink ID="HyperLink2" runat="server" CssClass="menu_reportes_borde" >--%>
                        <asp:HyperLink ID="lnkReports" runat="server" NavigateUrl="~/Modules/Reports/Dashboard.aspx" TabIndex="10"  
                            CssClass="menu_inicio_borde icono_menu icono_reportes ancho_item_menu" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label16" runat="server" Text="Reportes" meta:resourcekey="Label16Resource1" ></asp:Label>
                        </asp:HyperLink>
             </div>
            <div id="menu_finanzas">
                        <asp:HyperLink ID="lnkFinance" runat="server" NavigateUrl="~/Modules/Management/Accounting/AccountingDashboard.aspx" 
                            CssClass="menu_inicio_borde icono_menu icono_finanzas ancho_item_menu" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label13" runat="server" Text="Finanzas" meta:resourcekey="Label13Resource1" ></asp:Label>
                        </asp:HyperLink>
            </div>
            <div id="menu_recursos">
                        <asp:HyperLink ID="lnkRecursos" runat="server" NavigateUrl="~/Modules/RRHH/RRHHDashboard.aspx" 
                            CssClass="menu_inicio_borde icono_menu icono_recursos ancho_item_menu" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label8" runat="server" Text="RRHH" ></asp:Label>
                        </asp:HyperLink>
            </div>
            <div id="menu_sms">
                        <asp:HyperLink ID="lnkSMS" runat="server" NavigateUrl="~/Modules/SMS/SmsDashboard.aspx" 
                            CssClass="menu_inicio_borde icono_menu icono_sms ancho_item_menu" >
                            <i class="icono_espacio_menu"></i> 
                            <asp:Label ID="Label2" runat="server" Text="SMS" ></asp:Label>
                        </asp:HyperLink>
            </div>
             <div id="menu_datos">
                <asp:Label ID="Label9" runat="server" Text="" Width="100px"></asp:Label>
                <asp:Label ID="lblDateTime" runat="server" Text="" ></asp:Label>
                <br />
                <asp:Label ID="Label10" runat="server" Text="" Width="130px"></asp:Label>
                <asp:HyperLink ID="lnkExchangeRate" runat="server" NavigateUrl="~/Modules/Management/Accounting/ExchangeRate.aspx">
                    <asp:Label ID="lblExchangeRate" runat="server" Text="0.00" Font-Bold="True" ForeColor="#CC00CC"></asp:Label>
                </asp:HyperLink>
                <asp:Label ID="lblSeparatorTC" runat="server" Text="│" ></asp:Label>
                <asp:HyperLink ID="lnkExchangeRateOficial" runat="server" NavigateUrl="~/Modules/Management/Accounting/ExchangeRateOficial.aspx">
                    <asp:Label ID="lblExchangeRateOficial" runat="server" Text="0.00" Font-Bold="True" ForeColor="#00CCFF"></asp:Label>
                </asp:HyperLink>

            </div>
            </div>


            <!-- / Menu Principal anterior -->
            <div class="tabs_lateral_contenido" style="margin-left:30px;">
                <div class="tabs_contenido">

                <%--<div style="padding: 10px;">
                <asp:Image ID="imgLogoGanoLife2" runat="server" 
                    ImageUrl="~/Styles/2015/img/logo.png" ToolTip="Logo GanoLife" />
                </div>--%>
                
                <div class="tab_panel active" id="tab_menu_principal">
                <!-- Menu Principal Izquierda-->


                <nav id="menu_izquierda" class="ocultar_en_pc222"  runat="server" style="height: 66px!important; display:none;">
                <ul id="menu_principal_visible"  runat="server">

                        <ul>
                        <li>
                        <asp:HyperLink ID="lnkCRMCustomers" runat="server" 
                                NavigateUrl="~/Modules/CRM/CRMdashboard.aspx#top" CssClass="icono_menu icono_vacio" >
                                <i class="icono_espacio_menu"></i><asp:Label ID="Label92" runat="server" Text="- Clientes" 
                                meta:resourcekey="Label2Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        <li>
                        <asp:HyperLink ID="lnkCRMMarketing" runat="server" 
                                NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio" ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label93" runat="server" Text="- Marketing" 
                                meta:resourcekey="Label3Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        <li>
                        <asp:HyperLink ID="lnkCRMReports" runat="server" NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio" ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label94" runat="server" Text="- Reportes" 
                                meta:resourcekey="Label4Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        </ul>
                                    

                    <li id="menu_almacen2">
                        <asp:HyperLink ID="lnkWarehouse" runat="server" Visible="false" 
                            NavigateUrl="~/Modules/Inventory/Home.aspx#top" CssClass="menu_almacen_borde icono_menu icono_pedidos" >
                        <i class="icono_espacio_menu"></i> <asp:Label ID="Label96" runat="server" 
                            Text="Almacén e Inventario" meta:resourcekey="Label6Resource1" ></asp:Label>
                        </asp:HyperLink>
<%--                        <ul>
                        <li>
                        <asp:HyperLink ID="lnkWarehouseManagment" runat="server" 
                                NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio" ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label7" runat="server" Text="- Almacén" meta:resourcekey="Label7Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        <li>
                        <asp:HyperLink ID="lnkWarehouseProducts" runat="server" 
                                NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio"  ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label8" runat="server" Text="- Productos" 
                                meta:resourcekey="Label8Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        <li>
                        <asp:HyperLink ID="lnkWarehouseOrders" runat="server" 
                                NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio" ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label9" runat="server" Text="- Pedidos" meta:resourcekey="Label9Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        <li>
                        <asp:HyperLink ID="lnkWarehouseReports" runat="server" 
                                NavigateUrl="~/dashboard.aspx#top" CssClass="icono_menu icono_vacio" ><i class="icono_espacio_menu"></i><asp:Label 
                                ID="Label10" runat="server" Text="- Reportes" 
                                meta:resourcekey="Label10Resource1" ></asp:Label>
</asp:HyperLink>
                        </li>
                        </ul>--%>
                    </li>

                    

               <%--     <li id="menu_fabricacion">
                        <asp:HyperLink ID="lnkMRP" runat="server" 
                            NavigateUrl="~/Modules/Inventory/InventoryDashboard.aspx#top" 
                            CssClass="menu_fabricacion_borde icono_menu icono_fabricacion" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label15" runat="server" Text="Gestión de  Inventarios" 
                            meta:resourcekey="Label15Resource1" ></asp:Label>
                        </asp:HyperLink>
                    </li>--%>

                <%--    <li id="menu_almacen">
                        <asp:HyperLink ID="HyperLink6" runat="server" 
                            NavigateUrl="~/Modules/CDA/CDADashboard.aspx#top" 
                            CssClass="menu_almacen_borde icono_menu icono_cda" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label2" runat="server" Text="Centros de Apoyo (CDA)" ></asp:Label>
                        </asp:HyperLink>
                    </li>--%>
                    
          <%--          <li id="menu_ewallet" >
                        <asp:HyperLink ID="lnkPOS" runat="server" NavigateUrl="~/Modules/Ewallet/EwalletDashboard.aspx#top" 
                            CssClass="menu_ewallet_borde icono_menu icono_ewallet" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label12" runat="server" Text="EWallet" ></asp:Label>
</asp:HyperLink>
                    </li>--%>

                    <li id="menu_humanos">
                        <asp:HyperLink ID="lnkRRHH" runat="server" NavigateUrl="~/dashboard.aspx#top" Visible="true"
                            CssClass="menu_humanos_borde icono_menu icono_recursos"><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label14" runat="server" Text="Recursos Humanos" 
                            meta:resourcekey="Label14Resource1" ></asp:Label>
</asp:HyperLink>
                    </li>

                    <li id="menu_compras">
                        <asp:HyperLink ID="lnkPurchases" runat="server" Visible="false"
                            NavigateUrl="~/dashboard.aspx#top" 
                            CssClass="menu_compras_borde icono_menu icono_compras" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label11" runat="server" Text="Compras" meta:resourcekey="Label11Resource1" ></asp:Label>
                        </asp:HyperLink>
                    </li>
                             


                   <%-- <li id="menu_email">
                        <asp:HyperLink ID="HyperLink1" runat="server" 
                            NavigateUrl="http://www.ganolife.pe/Correo/" Target="_blank"  
                            CssClass="menu_email_borde icono_menu icono_contacto" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label19" runat="server" Text="Email" meta:resourcekey="Label19Resource1" ></asp:Label>
</asp:HyperLink>
                    </li>--%>

          <%--          <li id="menu_nube">
                        <asp:HyperLink ID="HyperLink2" runat="server" NavigateUrl="~/Cloud.aspx#top" 
                            CssClass="menu_nube_borde icono_menu icono_nube" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label20" runat="server" Text="Mi Nube" meta:resourcekey="Label20Resource1" ></asp:Label>
</asp:HyperLink>
                    </li>--%>
                 
                 <%--   <li id="menu_configuracion">
                        <asp:HyperLink ID="lnkTools" runat="server" NavigateUrl="~/Modules/Management/ManagementDashboard.aspx#top"  
                            CssClass="menu_configuracion_borde icono_menu icono_administracion" ><i class="icono_espacio_menu"></i> <asp:Label 
                            ID="Label17" runat="server" Text="Gerencia" 
                            meta:resourcekey="Label17Resource1" ></asp:Label>
</asp:HyperLink>
                    </li>--%>

     <%--                <li id="menu_seguridad">
                        <asp:HyperLink ID="lnkSecurity" runat="server"  
                             NavigateUrl="~/Modules/Security/User.aspx#top" 
                             CssClass="menu_seguridad_borde icono_menu icono_seguridad" ><i class="icono_espacio_menu"></i> <asp:Label 
                             ID="Label18" runat="server" Text="Usuario" 
                             meta:resourcekey="Label18Resource1" ></asp:Label>
</asp:HyperLink>
                    </li>--%>


                </ul>
                </nav>
                <!-- /Menu Principal Izquierda-->


                <br>

                </div>


                </div>
            </div>



            </td>
            </tr>
</table>





<aside id="pagina_barra_lateral" runat="server"  >
        <div >
            <!-- Mini logo -->
            <%--<div class="logo_modulo" >
                <a href="#">
                <asp:Image ID="Image2" runat="server" ImageUrl="~/Styles/2015/img/logo_365.png" ToolTip="Logo 365"/>
                </a>
            </div>--%>
            <!-- /Mini logo -->
        </div>
</aside>
<!-- /Contenido total lado  izquierda -->



    </ContentTemplate>
    </asp:UpdatePanel>


<asp:UpdatePanel ID="upPopupShoppingCar" runat="server">
<ContentTemplate>

     <!-- Popup Proximamente -->

</ContentTemplate>
</asp:UpdatePanel>




<asp:UpdatePanel ID="upMenu2" runat="server">
<ContentTemplate>

    <!-- /Menu Tiles Principal -->
    <div id="centrado" runat="server" class="ocultar_menu_tiles">

        <div id="fondo_menu_tablet" runat="server"  >


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_inicio" >
            <asp:HyperLink ID="hlnkMenuInicio" runat="server" NavigateUrl="~/Dashboard.aspx#top" >
            <div runat="server" class="icono_inicio_tablet"></div>
            <div runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuInicio" runat="server" Text="Dashboard" meta:resourcekey="hlblMenuInicioResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_crm" >
            <asp:HyperLink ID="hlnkMenuCRM" runat="server" NavigateUrl="~/Modules/CRM/CRMdashboard.aspx#top" >
            <div runat="server" class="icono_crm_tablet"></div>
            <div runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuCRM" runat="server" Text="CRM" meta:resourcekey="hlblMenuCRMResource1"></asp:Label>
            </div>
            </asp:HyperLink>
            </div>


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_ventas">
            <asp:HyperLink ID="hlnkMenuSales" runat="server" NavigateUrl="~/Modules/Orders/OrderDashboard.aspx#top"  >
            <div id="Div1" runat="server" class="icono_distribuidores_tablet"></div>
            <div id="Div4" runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuSales"  runat="server" Text="Ventas / Pedidos" meta:resourcekey="hlblMenuSalesResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_sucursales">
            <asp:HyperLink ID="hlnkBranchOffice" runat="server" NavigateUrl="~/Modules/WarehouseManager/Home.aspx#top" >
            <div id="Div8" runat="server" class="icono_sucursales_tablet"></div>
            <div id="Div9" runat="server" class="tile_informacion">
            <asp:Label ID="hlblBranchOffice" runat="server" Text="Entrega de Mercadería" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_reportes">
            <asp:HyperLink ID="hlnkMenuReports" runat="server" NavigateUrl="~/Modules/Reports/Dashboard.aspx#top" >
            <div id="Div10" runat="server" class="icono_reportes_tablet"></div>
            <div id="Div11" runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuReports"  runat="server" Text="Reportes" meta:resourcekey="hlblMenuReportsResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>




            <div id="Div5" class="tile_menu_tablet icono_menu_tablet boton_tablet_almacen" runat="server" Visible="false">
            <asp:HyperLink ID="hlnkMenuWarehouse" runat="server" NavigateUrl="~/Modules/Inventory/Home.aspx#top" >
            <div id="Div6" runat="server" class="icono_pedidos_tablet"></div>
            <div id="Div7" runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuWarehouse"  runat="server" Text="Almacén e Inventario" meta:resourcekey="hlblMenuWarehouseResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_compras" runat="server" Visible="false">
            <asp:HyperLink ID="hlnkMenuPurchases" runat="server" NavigateUrl="#top" CssClass="menu-link" >
            <div id="Div2" runat="server" class="icono_compras_tablet"></div>
            <div id="Div3" runat="server" class="tile_informacion">
            <asp:Label ID="hlblMenuPurchases" runat="server" Text="Compras" meta:resourcekey="hlblMenuPurchasesResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

<%--            <div id="target-content">
            <a href="#contenedor_de_pagina" class="close"></a>
            <div id="target-inner" > 
            <asp:Label ID="lblMenuCRM" runat="server" Text="CRM" 
                    meta:resourcekey="lblMenuCRMResource2" ></asp:Label><hr style="margin-top:0px;" >
                  <table  width="100%" border="0" align="center" cellpadding="6" cellspacing="0">
                  <tr>
                    <td align="center">
                    <asp:HyperLink ID="hlnkMenuCRMCustomers" runat="server" 
                            class="tile_menu_tablet boton_tablet_crmsub boton_zoom" 
                            style="width:90px!important; height:90px!important;" 
                            NavigateUrl="~/Modules/CRM/CRMdashboard.aspx#top" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlblMenuCRMCustomers" runat="server" Text="Clientes" 
                                meta:resourcekey="hlblMenuCRMCustomersResource1" ></asp:Label>
</div>
</asp:HyperLink>
     
                    <asp:HyperLink ID="hlnkMenuCRMMarketing" runat="server" 
                            class="tile_menu_tablet  boton_tablet_crmsub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlblMenuCRMMarketing" runat="server" Text="Marketing" 
                                meta:resourcekey="hlblMenuCRMMarketingResource1" ></asp:Label>
</div>
</asp:HyperLink>

                    <asp:HyperLink ID="hlnkMenuCRMReports" runat="server" 
                            class="tile_menu_tablet boton_tablet_crmsub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlblMenuCRMReports" runat="server" Text="Reportes" 
                                meta:resourcekey="hlblMenuCRMReportsResource1" ></asp:Label>
</div>
</asp:HyperLink>
                    </td>
                  </tr>
                  </table>
            </div>
            </div>--%>

<%--            <div id="target-content2">
            <a href="#contenedor_de_pagina" class="close"></a>
            <div id="target-inner2" > 
            <asp:Label ID="lblMenuWarehouse" runat="server" Text="Almacén e Inventario" 
                    meta:resourcekey="lblMenuWarehouseResource2" ></asp:Label><hr style="margin-top:0px;" >
                  <table  width="100%" border="0" align="center" cellpadding="6" cellspacing="0">
                  <tr>
                    <td align="center">
                    <asp:HyperLink ID="hlnkMenuWarehouseManagment" runat="server" 
                            class="tile_menu_tablet boton_tablet_almacensub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlbkMenuWarehouseManagment" runat="server" Text="Almacén" 
                                meta:resourcekey="hlbkMenuWarehouseManagmentResource1" ></asp:Label>
</div>
</asp:HyperLink>
     
                    <asp:HyperLink ID="hlnkMenuWarehouseProducts" runat="server" 
                            class="tile_menu_tablet  boton_tablet_almacensub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlbkMenuWarehouseProducts" runat="server" Text="Productos" 
                                meta:resourcekey="hlbkMenuWarehouseProductsResource1" ></asp:Label>
</div>
</asp:HyperLink>

                    <asp:HyperLink ID="hlnkMenuWarehouseOrders" runat="server" 
                            class="tile_menu_tablet boton_tablet_almacensub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlbkMenuWarehouseOrders" runat="server" Text="Pedidos" 
                                meta:resourcekey="hlbkMenuWarehouseOrdersResource1" ></asp:Label>
</div>
</asp:HyperLink>

                    <asp:HyperLink ID="hlnkMenuWarehouseReports" runat="server" 
                            class="tile_menu_tablet boton_tablet_almacensub boton_zoom" 
                            style="width:90px!important; height:90px!important;" NavigateUrl="#" ><div runat="server" class="submenu_crm"><asp:Label 
                                ID="hlbkMenuWarehouseReports" runat="server" Text="Reportes" 
                                meta:resourcekey="hlbkMenuWarehouseReportsResource1" ></asp:Label>
</div>
</asp:HyperLink>

                    </td>
                  </tr>
                  </table>
            </div>
            </div>--%>
            

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_pos" runat="server" Visible="false">
            <asp:HyperLink ID="hlnkMenuPOS" runat="server" NavigateUrl="#top" 
                    CssClass="menu-link" ><div runat="server" class="icono_pos_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuPOS" 
                    runat="server" Text="POS" meta:resourcekey="hlblMenuPOSResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_finanzas" runat="server" >
            <asp:HyperLink ID="hlnkMenuFinance" runat="server" NavigateUrl="~/Modules/Management/Accounting/AccountingDashboard.aspx" CssClass="menu-link" >
            <div runat="server" class="icono_finanzas_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuFinance" 
                    runat="server" Text="Finanzas" meta:resourcekey="hlblMenuFinanceResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_seguridad">
            <asp:HyperLink ID="hlnkMenuSms" runat="server" NavigateUrl="~/Modules/SMS/SmsDashboard.aspx">
            <div id="Div13" runat="server" class="icono_sms_tablet"></div>
            <div id="Div14" runat="server" class="tile_informacion">
                <asp:Label ID="Label7" runat="server" Text="SMS" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_rrhh" runat="server" Visible="true">
            <asp:HyperLink ID="hlnkMenuRRHH" runat="server" NavigateUrl="#top" 
                    CssClass="menu-link" ><div runat="server" class="icono_rrhh_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuRRHH" 
                    runat="server" Text="Recursos Humanos" 
                    meta:resourcekey="hlblMenuRRHHResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>


            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_fabricacion" runat="server" Visible="false" >
            <asp:HyperLink ID="hlnkMenuMRP" runat="server" NavigateUrl="~/Modules/Inventory/InventoryDashboard.aspx#top" 
                    CssClass="" ><div runat="server" class="icono_fabricacion_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuMRP" 
                    runat="server" Text="Gestión de  Inventarios" meta:resourcekey="hlblMenuMRPResource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_cda" runat="server" Visible="false">
            <asp:HyperLink ID="HyperLink8" runat="server" NavigateUrl="~/Modules/CDA/CDADashboard.aspx#top" 
                    CssClass="" ><div runat="server" class="icono_cda_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="Label3" runat="server" Text="Centros de Apoyo (CDA)"></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_ewallet" runat="server" Visible="false" >
            <asp:HyperLink ID="HyperLink9" runat="server" NavigateUrl="~/Modules/Ewallet/EwalletDashboard.aspx#top" 
                    CssClass="" ><div runat="server" class="icono_ewallet_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="Label4" runat="server" Text="Créditos E-Wallet" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_reportes" runat="server" Visible="false">
            <asp:HyperLink ID="HyperLink3" runat="server" 
                    NavigateUrl="http://www.ganolife.pe/Correo/" Target="_blank" ><div runat="server" class="icono_contacto_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="Label21" runat="server" 
                    Text="Email" meta:resourcekey="Label21Resource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_reportes" runat="server" Visible="false">
            <asp:HyperLink ID="HyperLink4" runat="server" NavigateUrl="~/Cloud.aspx#top" ><div runat="server" class="icono_nube_tablet"></div>
            <div runat="server" class="tile_informacion"><asp:Label ID="Label22" runat="server" 
                    Text="Entrega de Pedidos" meta:resourcekey="Label22Resource1" ></asp:Label>
            </div>
            </asp:HyperLink>
            </div>

 
            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_herramientas" runat="server" Visible="false" >
            <asp:HyperLink ID="hlnkMenuTools" runat="server" NavigateUrl="~/Modules/Management/ManagementDashboard.aspx#top" ><div runat="server" class="icono_administracion_tablet"></div>
<div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuTools" 
        runat="server" Text="Gerencia" meta:resourcekey="hlblMenuToolsResource1" ></asp:Label>
</div>
</asp:HyperLink>
            </div>
           
            <div class="tile_menu_tablet icono_menu_tablet boton_tablet_seguridad" runat="server" Visible="false" >
            <asp:HyperLink ID="hlnkSecurity" runat="server"  NavigateUrl="~/Modules/Security/User.aspx#top" ><div runat="server" class="icono_seguridad_tablet"></div>
<div runat="server" class="tile_informacion"><asp:Label ID="hlblMenuSecurity" 
        runat="server" Text="Usuario" meta:resourcekey="hlblMenuSecurityResource1" ></asp:Label>
</div>
</asp:HyperLink>
            </div>


        </div>

    </div>
    <!-- /Menu Tiles Principal -->

</ContentTemplate>
</asp:UpdatePanel>


<!-- Contenido -->
<div id="contenido_de_pagina2" >


    <!-- Bloque -->
    <div class="fila-ajustable" >


        <!-- Contenido 1 -->
        <div class="columna_ancho12">


            <!-- Titulo de paginas -->
           <%-- <div style="margin-top:20px">
            <h2><asp:Label ID="lblTituloPagina" runat="server" ForeColor="#515151" Text="Home - Dashboard"></asp:Label></h2>    
            </div>--%>

            <!-- Indicador de posicion para menu tablet -->
            <div class="colocar_derecha" style="margin-right:50px; ">
            <a href="#" >
            <asp:Image ID="imgUserPhoto" runat="server" ImageUrl="~/Styles/2015/img/icono_menu3.png" ToolTip="Mostrar menu" 
                    CssClass="ver_menu_tiles" meta:resourcekey="imgUserPhotoResource1"  /> 
            </a>
            </div>


            <!-- Titulo oculto -->
            <%--<div id="titulo-usuario" style="display:none;">
            <h1>
            <asp:Label ID="lblTituloUsuario" runat="server" Text="Bienvenido"></asp:Label>
            </h1>
            </div>--%>

            <asp:Label ID="Linea_Home" runat="server" meta:resourcekey="Linea_HomeResource1"></asp:Label>

            <!-- Submenu oculto -->
            <div class="header2 ocultar" id="header2">

<%--            <div style="padding:10px 25px; float:left;">
            <div class="pix_diapo">
                <div>
                    <asp:HyperLink ID="lnkBanner01" runat="server" NavigateUrl="#" ToolTip="Publicidad">
                    <img src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/banner-slider/images/ganolife-banner-slide01.jpg' width="1150" height="150">
                    </asp:HyperLink>
                </div>
                <div>
                    <asp:HyperLink ID="lnkBanner02" runat="server" NavigateUrl="#" ToolTip="Publicidad">
                    <img src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/banner-slider/images/ganolife-banner-slide02.jpg' width="1150" height="150">
                    </asp:HyperLink>
                </div>
                <div>
                    <asp:HyperLink ID="lnkBanner03" runat="server" NavigateUrl="#" ToolTip="Publicidad">
                    <img src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/banner-slider/images/ganolife-banner-slide03.jpg' width="1150" height="150">
                    </asp:HyperLink>
                </div>
			</div> 
            </div>--%>

            <nav id="submenu-inferior">
            	<%--<p style="text-align:left; font-size:20px;color:#FFF;margin:0;padding:0;">SUBMENU*</p>--%>
                <%--<uc1:wucSubMenu ID="wucSubMenu1" runat="server" />--%>
            </nav>

            </div>


        </div>


    </div>

</div>



<!-- /Contenedor principal -->


</div>




<div class="main" >


     <asp:ContentPlaceHolder ID="MainContent" runat="server"/>



</div>


<br>

<asp:UpdatePanel ID="upFooter" runat="server">
<ContentTemplate>

<div class="footer" style="margin-top: -20px">

<!-- Contenedor principal -->
<div id="contenedor_de_pagina2" class="ancho_de_pagina">



<!-- Footer -->
<footer  style="background-color: #f1f1f1" >

<table width="100%" height="100%" border="0" align="center" cellpadding="4" cellspacing="0" style=" background-color:#f1f1f1;">
  <tr>
    <td width="3%"> 
    </td>
    <td width="61%" valign="top" align="left"> 
        <div class="colocar_izquierda">
        <asp:Label ID="lblDerechosReservados" runat="server" 
                Text="2017 Ganolife - Derechos Reservados" 
                meta:resourcekey="lblDerechosReservadosResource1"></asp:Label>
        </div>
        <br>
        <div class="colocar_izquierda">
        <asp:HyperLink ID="lnkPrivacidad" runat="server" TabIndex="20" 
                NavigateUrl="~/PrivacyPolicy.aspx#top" ForeColor="#343432" 
                CssClass="piepag_link" ToolTip="Políticas de Privacidad" 
                meta:resourcekey="lnkPrivacidadResource1">Políticas de Privacidad</asp:HyperLink>
        |
        <%--<asp:HyperLink ID="lnkTerminos" runat="server" TabIndex="21"  NavigateUrl="~/TermsofUse.aspx#top" 
                ForeColor="#343432" CssClass="piepag_link" ToolTip="Términos de Uso" 
                meta:resourcekey="lnkTerminosResource1">Términos de Uso</asp:HyperLink>
        |--%>
        <asp:HyperLink ID="lnkCondiciones" runat="server" TabIndex="22" 
                NavigateUrl="~/TermsandConditions.aspx#top" ForeColor="#343432" 
                CssClass="piepag_link" ToolTip="Términos y Condiciones" 
                meta:resourcekey="lnkCondicionesResource1">Términos y Condiciones</asp:HyperLink>
        |
        <asp:HyperLink ID="lnkContactenos" runat="server" TabIndex="23" 
                NavigateUrl="~/ContactUs.aspx#top" ForeColor="#343432" CssClass="piepag_link" 
                ToolTip="Contáctenos" meta:resourcekey="lnkContactenosResource1">Contáctenos</asp:HyperLink>
        <%--|
        <asp:HyperLink ID="lnkPreguntas" runat="server" NavigateUrl="~/Faq.aspx#top" ForeColor="#343432" CssClass="piepag_link" ToolTip="Preguntas Frecuentes">Preguntas Frecuentes</asp:HyperLink>
        |
        <asp:HyperLink ID="lnkMapa" runat="server" NavigateUrl="~/SiteMap.aspx#top" ForeColor="#343432" CssClass="piepag_link" ToolTip="Mapa de sitio">Mapa de sitio</asp:HyperLink>--%>
        </div>
    </td>

    <td width="5%"> 
    </td>

    <td width="28%" valign="top" align="right"><!-- Social -->
        <div class="colocar_derecha" id="social">
        
        <asp:HyperLink ID="lnkSocialFacebook" runat="server" 
                NavigateUrl="https://www.facebook.com/Ganolife.Sitio.Oficial" 
                CssClass="facebook" ToolTip="facebook" Target="_blank" 
                meta:resourcekey="lnkSocialFacebookResource1"> <asp:Image ID="imgFacebook" 
                runat="server" ImageUrl="~/Styles/2015/img/icono_facebook.png" 
                meta:resourcekey="imgFacebookResource1" />
        
</asp:HyperLink>
        
        <asp:HyperLink ID="lnkSocialYoutube" runat="server" 
                NavigateUrl="http://www.youtube.com/user/ganolifeint/" CssClass="youtube" 
                ToolTip="youtube" Target="_blank" meta:resourcekey="lnkSocialYoutubeResource1"> <asp:Image 
                ID="imgYoutube" runat="server" ImageUrl="~/Styles/2015/img/icono_youtube.png" 
                meta:resourcekey="imgYoutubeResource1" />
        
</asp:HyperLink>
        
        <asp:HyperLink ID="lnkSocialTwiter" runat="server" 
                NavigateUrl="http://twitter.com/GanoLifePeru/" CssClass="twitter" 
                ToolTip="twitter" Target="_blank" meta:resourcekey="lnkSocialTwiterResource1"> <asp:Image 
                ID="imgTwitter" runat="server" ImageUrl="~/Styles/2015/img/icono_twitter.png" 
                meta:resourcekey="imgTwitterResource1" />
        
</asp:HyperLink>

        <br /><asp:Label ID="lblText1" runat="server" Text="Desarollado por: " 
                meta:resourcekey="lblText1Resource1" ></asp:Label><asp:Label ID="lblText2" 
                runat="server" Text="Área de Sistemas Ganolife" Font-Bold="True" 
                meta:resourcekey="lblText2Resource1" ></asp:Label>

        </div>

    </td>
    <td width="3%"> 
    </td>


  </tr>
</table>

</footer>
<!-- /Footer -->


</div>
<!-- /Contenedor principal -->


</div>





<script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/2015/menu/js/classie.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"]%>'></script>
<script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/2015/menu/js/sidebarEffects.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"]%>'></script>





</div>
<!-- /Total -->

</ContentTemplate>
</asp:UpdatePanel>


    </form>


    <script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/2015/js/vendor/bootstrap.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/2015/js/plugins.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type='text/javascript' src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/2015/js/main.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>



</body>
</html>

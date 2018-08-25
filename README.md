<%@ Master Language="C#" AutoEventWireup="true" CodeFile="Site.Master.cs" Inherits="SiteMaster" %>



<!DOCTYPE html>
<html lang="en">
<head>

<meta charset="utf-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Zarpe con nosotros</title>
<link rel="shortcut icon" type="image/png" href="https://www.zar.pe/descargas/Imagenes/favicon.png"/>
<%--<meta name="description" content="La plataforma que le ayudará a hacer crecer su negocio está aquí. Ingrese hoy y comparta nuestro contenido con todos para llegar más lejos." />--%>
<meta name="keywords" content="zarpe, zarpe con nosotros, bienestar, salud, vida sana, emprendimiento, ganoderma,  ganoderma 365, ganoderma lucidum, hongo, hongo chino, super alimentos, latte, black, latte 365, black 365, atp, atp 365, reset, reset 365, medicina tradicional asiática , shelf mushroom, bracket fungus, conk funguss, hongo narigon, fungi, ganodermataceae, reishi, lingzhi, hongo milenario, Maca, guaraná, cordyceps, bebida energética, Rosa de Jamaica, Hibiscus sabdariffa, Flor de Jamaica, Roselle, café, café saludable, rutina, fórmula perfecta, bebida saludable" />
<%--<link rel="canonical" href="https://www.zar.pe/" /> --%>


    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/css/main.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/css/patch.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/flag-icon-css/css/flag-icon.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/bootstrap-drawer/dist/css/bootstrap-drawer.min.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/slick-carousel/slick/slick.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/slick-carousel/slick/slick-theme.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/bootstrap/dist/css/bootstrap.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>

    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/PopupDialog.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.toastmessage-min.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
    <%-- SLider --%>
    <%--<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/slider/hwslider.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>--%>



    <%--<link href="https://fonts.googleapis.com/css?family=Shadows+Into+Light" rel="stylesheet" type="text/css">--%>

    <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700" rel="stylesheet">

    <!-- Parallax -->
    <link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/css/parallax.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>


    <!-- Slider comentarios -->
    <%--<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/css/slidezarpe.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
--%>





<!-- PopupMessage -->
<style>
.aparecer 
{
-webkit-animation-name: MiAnimacion; /* Chrome, Safari, Opera */
-webkit-animation-duration: 5s; /* Chrome, Safari, Opera */
/*-webkit-animation-delay: 10s;*/
animation-name: MiAnimacion;
animation-duration: 8s;
/*animation-delay: 10s;*/
}
/* Chrome, Safari, Opera */
@-webkit-keyframes MiAnimacion {
from {opacity: 0; bottom:-3000%;}
to {opacity: 1}
}
/* Standard syntax */
@keyframes MiAnimacion {
from {opacity: 0; bottom:-3000%;}
to {opacity: 1}
}



</style>



    <asp:ContentPlaceHolder ID="HeadContent" runat="server">


    </asp:ContentPlaceHolder>

    </head>
    <body class="has-drawer">


    <form id="Form1" runat="server">


    <%-- GENERAL --%>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery-1.11.3.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery-ui-1.10.3.custom.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.blockUI.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>


<%--    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/bower_components/jquery/dist/jquery.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>--%>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/bootstrap/dist/js/bootstrap.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/bootstrap-drawer/dist/js/drawer.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/bower_components/slick-carousel/slick/slick.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/js/app.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>


<%--    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.alerts.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/alertify.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>--%>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.bpopup.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
<%--    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.quicksearch.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.numeric.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>--%>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.toastmessage-min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General/jquery.quicksearch.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/General.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/MasterPage.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>
    <script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Scripts/Services.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>

<script>

    $.ajax({
        url: 'https://api.ipstack.com/check?access_key=27feae6f49366d628feaf371f8edc3f4',
        dataType: 'jsonp',
        success: function (json) {
            //alert(json.country_name);
            var hdCountryForLocation = document.getElementById("hdCountryForLocation");
            var btnCountryForLocation = document.getElementById("btnCountryForLocation");

            hdCountryForLocation.value = json.country_name;
            btnCountryForLocation.click();
        }
    });

</script>




<!-- Carusel Menu / Items  -->
<%--<link type="text/css" media="all" href="slide/slide2222222.css" rel="stylesheet" />
<script type='text/javascript' src='slide/jquery222222.js'></script>--%>
<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/slide2.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
<script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/jquery.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>



<!--[if lte IE 9]><link rel="stylesheet" type="text/css" href="http://www.masterslider.com/wp-content/plugins/js_composer/assets/css/vc_lte_ie9.min.css" media="screen"><![endif]-->	


<%--<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/css/slidezarpe.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>--%>

<%--<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/sticky.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/style.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>
<link rel="stylesheet" href='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/pure-js-carousel.css<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'>

--%>




<asp:HiddenField ID="hdCountryForLocation" runat="server" ClientIDMode="Static" />
<asp:Button ID="btnCountryForLocation" runat="server" ClientIDMode="Static" onclick="btnCountryForLocation_Click" style="display:none;" />


    <asp:ScriptManager ID="ToolkitScriptManager1" runat="server" EnableScriptGlobalization="True" AsyncPostBackTimeout="120000" ScriptMode="Release" />



<asp:UpdatePanel ID="upPopups" runat="server">
<ContentTemplate>

<!-- PopupMessage -->
<div id="popupMessageShippingFree" runat="server" visible="false"
     class="aparecer" style="background-color: #a4cde1; bottom:0px; position:fixed; width:100%; z-index:99998; padding:0px; ">
    <table width="94%" border="0" align="center" cellpadding="0" cellspacing="0" >
    <tr>
    <td > 
    <div style="float:right; padding-right:15px;">
    <asp:ImageButton ID="imgShippingFreeClose" runat="server" ImageUrl="~/Styles/images/zarpe_x3.png" 
    OnClientClick="$('#popupMessageShippingFree').bPopup().close();" style="width:100%; max-width:30px; " />
    </div>
    </td>
    </tr>
    <tr>
    <td align="center" >
    <asp:LinkButton ID="lnkShippingFreeSales" runat="server" OnClick="lnkShippingFreeSales_Click" style="text-decoration:none; ">
    <asp:Image ID="imgShippingFreeSales" runat="server" ImageUrl="~/Styles/images/popup_compra_1.jpg" style="width:90%; display:none; "/>
    <asp:Label ID="Label64" runat="server" ForeColor="#001E3A" Text="ENVÍO TOTALMENTE ¡GRATIS! EN ÓRDENES SUPERIORES A US$50" 
    CssClass="texto_6b" ></asp:Label>
    <br>
    <div style="background: #ffffff; margin:10px; padding:9px; width:210px!important; border-radius:30px; text-decoration:none; 
    color:#001E3A; width:70%; " class="texto_3">
    <asp:Label ID="Label65" runat="server" ForeColor="#001E3A" Text="¡ORDENAR AHORA!" CssClass="texto_6b" ></asp:Label>
    </div>

    </asp:LinkButton>

<%--    <asp:LinkButton ID="lnkShippingFreeClose" runat="server" OnClientClick="$('#popupMessageShippingFree').bPopup().close();">--%>
    

    
<%--    </asp:LinkButton>--%>
    </td>
    </tr>
    </table>
</div>

<!-- PopupMessage GetProductDiscount -->
<div id="popupMessageGetProductDiscount" runat="server" visible="false" 
    class="aparecer" style="background-color: #a4cde1; bottom:0px; position:fixed; width:100%; z-index:99999; padding:0px; ">
    <table width="94%" border="0" align="center" cellpadding="0" cellspacing="0" >
    <tr>
    <td>
    <div style="float:right; padding-right:15px;">
    <asp:ImageButton ID="imgGetProductDiscountClose" runat="server" ImageUrl="~/Styles/images/zarpe_x3.png" 
    OnClientClick="$('#popupMessageGetProductDiscount').bPopup().close();" style="width:100%; max-width:30px; " />
    </div>
    </td>
    </tr>
    <tr>
    <td align="center" >
    <asp:LinkButton ID="lnkGetProductDiscount" runat="server" OnClientClick="$('#pnlGetProductDiscount').bPopup().show(); return false;" style="text-decoration:none; ">
    <asp:Image ID="imgGetProductDiscountSales" runat="server" ImageUrl="~/Styles/images/popup_compra_1.jpg" style="width:90%; display:none; "/>
    <asp:Label ID="Label67" runat="server" ForeColor="#001E3A" Text="¿Deseas ahorrar hasta el 40% de descuento en nuestros productos?" CssClass="texto_6b" ></asp:Label>
    <br>
    <div style="background: #ffffff; margin:10px; padding:9px; width:210px!important; border-radius:30px; text-decoration:none; 
    color:#001E3A; width:70%; " class="texto_3">
    <asp:Label ID="Label68" runat="server" ForeColor="#001E3A" Text="¡ENTÉRATE CÓMO!" CssClass="texto_6b" ></asp:Label>
    </div>

    </asp:LinkButton>

<%--    <asp:LinkButton ID="lnkGetProductDiscountClose" runat="server" OnClientClick="$('#popupMessageGetProductDiscount').bPopup().close();">
    </asp:LinkButton>--%>
    </td>
    </tr>
    </table>
</div>



    <!-- POPUP DESCUENTO EN PRODUCTOS -->
<%--    <asp:HiddenField ID="hdGetProductDiscount" runat="server" ClientIDMode="Static" />
    <asp:ModalPopupExtender ID="mpeGetProductDiscount" BehaviorID="mpeGetProductDiscount" runat="server" ClientIDMode="Static" BackgroundCssClass="modalBackground2" 
        PopupControlID="pnlGetProductDiscount" TargetControlID="hdGetProductDiscount" CancelControlID="lnkGetProductDiscountCancel" >
    </asp:ModalPopupExtender>--%>

    <asp:Panel ID="pnlGetProductDiscount" runat="server" ClientIDMode="Static" CssClass="PopupStyle popup_ancho" style="text-align:center; height:auto;">

    <asp:HiddenField ID="hdGetProductDiscountID" runat="server" Visible="false" />
    <table width="100%" border="0" align="center" cellpadding="5" cellspacing="0" style="background-color: #ffffff; padding:7px; border-radius:6px;">
        <tr>
        <td align="center">

            <br>
            <h4>
            <asp:Label ID="Label80" runat="server" Text="Ahorra mucho más en tus compras de producto ZARPE." ForeColor="#001e3a"></asp:Label>
            </h4>

            </td>
        </tr>
        <tr>
        <td style="padding: 30px;" align="left">

            <div style="height: 220px; overflow-y: scroll;" >

            <asp:Label ID="Label69" runat="server" Text="¿Que tienes que hacer?" ForeColor="#001e3a"></asp:Label>
            <br /><asp:Label ID="Label82" runat="server" Text="Al comprar un paquete mayorista o afiliarte a nuestro programa de suscripción mensual, accedes a precios de productos descontados (hasta un 40%) en tus compras siempre." ForeColor="#001e3a"></asp:Label>

            <br /><br />
            <asp:Label ID="Label83" runat="server" Text="¿Cómo funciona?" ForeColor="#001e3a"></asp:Label>
            <br /><asp:Label ID="Label84" runat="server" Text="Compra un paquete mayorista o subscribete a nuestro programa con una compra de US$100 en valor de producto y automáticamente conviértete en un afiliado y te entregaremos lo siguiente:" ForeColor="#001e3a"></asp:Label>

            <br /><br />
            <asp:Label ID="Label85" runat="server" Text="En un paquete mayorista 4 unidades de tu elección de los productos de Zarpe." ForeColor="#001e3a"></asp:Label>
            <br /><asp:Label ID="Label86" runat="server" Text="En una Suscripción Mensual te entregaremos 5 unidades de tu elección (Siempre y cuando hagas tus compras todos los meses)." ForeColor="#001e3a"></asp:Label>

            <br /><br />
            <asp:Label ID="Label87" runat="server" Text="*Los Afiliados son personas que han comprado al menos una vez en los últimos 6 meses un paquete de US$100 dólares en una sola compra y por esto reciben un descuento en el precio de nuestros productos." ForeColor="#001e3a"></asp:Label>
            <br /><asp:Label ID="Label88" runat="server" Text="**Los afiliados suscritos a nuestro programa de compras (Al menos US$100 dólares), hacen un compromiso de comprar nuestros productos mensualmente y acceden a un descuento aún mayor!" ForeColor="#001e3a"></asp:Label>

            </div>

        </td>
        </tr>

        <tr style="height:120px;" align="center">
        <td>
        <hr />
        <br />

        <asp:LinkButton ID="lnkGetProductDiscount_ORV" onclick="lnkPackAdd_Click" runat="server" Width="294px" 
        style="display:inline-block; text-decoration:none!important; text-align: center;">
        <div style="background: #afcbe0 !important; margin:10px; padding:20px; padding-bottom:10px; padding-top:10px; border-radius:30px; text-decoration:none!important; ">
        <asp:Label ID="Label79" runat="server" ForeColor="#001e3a" CssClass="titulo_7" Text="Compra un Paquete de Suscripción" ></asp:Label>
        </div>
        </asp:LinkButton>

        <asp:LinkButton ID="lnkGetProductDiscount_X1" runat="server" onclick="lnkPackAdd_Click" Width="294px" 
        style="display:inline-block; text-decoration:none!important; text-align: center;">
        <div style="background: #afcbe0 !important; margin:10px; padding:20px; padding-bottom:10px; padding-top:10px; border-radius:30px; text-decoration:none!important; ">
        <asp:Label ID="Label70" runat="server" ForeColor="#001e3a" CssClass="titulo_7" Text="Compra un Paquete Mayorista" ></asp:Label>
        </div>
        </asp:LinkButton>


        </td>
        </tr>


    </table>

    </asp:Panel>




</ContentTemplate>
</asp:UpdatePanel>




<div class="wrapper-general">


<!-- Menu movil antiguo -->
<div id="drawerExample" class="drawer dw-xs-10 dw-sm-6 dw-md-4 fold" aria-labelledby="drawerExample">

    <div class="drawer-contents">
        <div class="drawer-heading">
            <h2 class="drawer-title"><asp:Image ID="imgLogoResponsive" runat="server" ImageUrl="~/Styles/images/GanoLife.png" alt="" /></h2>
        </div>
        <ul class="drawer-nav">
            <li role="presentation" class="nav-mov" id="liMenuHomeResponsive" runat="server">
                 <asp:HyperLink ID="lnkHomeResponsive" runat="server" NavigateUrl="~/Home_Zarpe.aspx">
                        <asp:Label ID="lbHomeResponsive" runat="server" Text="Home"></asp:Label>
                 </asp:HyperLink>
            </li>
            <li role="presentation" class="nav-mov" id="liMenuProfileResponsive" runat="server">
                 <asp:HyperLink ID="lnkProfileResponsive" runat="server" NavigateUrl="~/Zarpe/Profile_Zarpe.aspx">
                        <asp:Label ID="lbProfileResponsive" runat="server" Text="Mi Perfil"></asp:Label>
                 </asp:HyperLink>
            </li>
            <li role="presentation" class="nav-mov" id="liMenuSecretResponsive" runat="server">
                 <asp:HyperLink ID="lnkSecretResponsive" runat="server" NavigateUrl="~/Secret_Zarpe.aspx">
                        <asp:Label ID="lbSecretResponsive" runat="server" Text="Fórmula"></asp:Label>
                 </asp:HyperLink>
            </li>
            <li role="presentation" class="nav-mov" id="liMenuProductsResponsive" runat="server">
                <asp:HyperLink ID="lnkProductsResponsive" runat="server" NavigateUrl="~/Products_Zarpe.aspx">
                        <asp:Label ID="lbProductsResponsive" runat="server" Text="Productos"></asp:Label>
                 </asp:HyperLink>
            </li>
            <%--<li role="presentation" class="nav-mov" data-nav="formula" id="liMenuFormuleResponsive" runat="server">
                <asp:HyperLink ID="lnkFormuleResponsive" runat="server" NavigateUrl="~/Home.aspx#formula">
                        <asp:Label ID="lbFormuleResponsive" runat="server" Text="Fórmula"></asp:Label>
                 </asp:HyperLink>
            </li>--%>
            <%--<li role="presentation" class="nav-mov" data-nav="historia" id="liMenuHistoryResponsive" runat="server">
                <asp:HyperLink ID="lnkHistoryResponsive" runat="server" NavigateUrl="~/Home.aspx#historia">
                        <asp:Label ID="lbHistoryResponsive" runat="server" Text="Historia"></asp:Label>
                 </asp:HyperLink>
            </li>--%>
<%--            <li role="presentation" class="nav-mov" id="liMenuSecretResponsive" runat="server">
                <asp:HyperLink ID="lnkSecretResponsive" runat="server" NavigateUrl="~/Secret.aspx">
                        <asp:Label ID="lbSecretResponsive" runat="server" Text="Secreto"></asp:Label>
                 </asp:HyperLink>
            </li>
            <li role="presentation" class="nav-mov" id="li7" runat="server">
                <asp:HyperLink ID="HyperLink10" runat="server" NavigateUrl="~/Products.aspx">
                        <asp:Label ID="Label27" runat="server" Text="Productos"></asp:Label>
                 </asp:HyperLink>
            </li>--%>
            <li role="presentation" class="nav-mov" id="liMenuSuperResponsive" runat="server">
                <asp:HyperLink ID="lnkSuperResponsive" runat="server" NavigateUrl="~/SuperAlimentos_Zarpe.aspx">
                        <asp:Label ID="lbSuperResponsive" runat="server" Text="Súper Alimentos"></asp:Label>
                 </asp:HyperLink>
            </li>
<%--            <li role="presentation" class="nav-mov" id="li8" runat="server">
                <asp:HyperLink ID="lnkSuperResponsive" runat="server" NavigateUrl="~/.aspx">
                        <asp:Label ID="lbSuperResponsive" runat="server" Text=""></asp:Label>
                 </asp:HyperLink>
            </li>--%>
            <li role="presentation" class="nav-mov" id="liMenuOportunityResponsive" runat="server">
                <asp:HyperLink ID="lnkOportunityResponsive" runat="server" NavigateUrl="~/Opportunity_Zarpe.aspx">
                        <asp:Label ID="lbOportunityResponsive" runat="server" Text="Oportunidad"></asp:Label>
                 </asp:HyperLink>
            </li>

            <li role="presentation" class="nav-mov" id="li1" runat="server">
                <div style="margin-left:15px;">
                        <asp:Label ID="Label14" runat="server" ForeColor="#777777" Text="Zarpe"></asp:Label>
                 </div>

                <ul style="margin-left:-20px; ">
                <li id="liMenuZarpe_HomeZarpeResponsive" runat="server">
                    <asp:HyperLink ID="lnkZarpe_HomeZarpeResponsive" runat="server" NavigateUrl="~/Zarpe/Home_Zarpe.aspx">- 
                    <asp:Label ID="lbZarpe_HomeZarpeResponsive" runat="server" Text="Home"></asp:Label> </asp:HyperLink></li>


                <li id="liMenuZarpe_DashboardZarpeResponsive" runat="server">
                    <asp:HyperLink ID="lnkZarpe_DashboardZarpeResponsive" runat="server" NavigateUrl="~/Zarpe/Dashboard_Zarpe.aspx">- 
                    <asp:Label ID="lbZarpe_DashboardZarpeResponsive" runat="server" Text="Tablero de Control"></asp:Label> </asp:HyperLink></li>

                <li id="liMenuZarpe_ProfileZarpeResponsive" runat="server">
                    <asp:HyperLink ID="lnkZarpe_ProfileZarpeResponsive" runat="server" NavigateUrl="~/Zarpe/Profile_Zarpe.aspx">- 
                    <asp:Label ID="lbZarpe_ProfileZarpeResponsive" runat="server" Text="Influenciador"></asp:Label> </asp:HyperLink></li>

                <li id="liMenuZarpe_First10HomeZarpeResponsive" runat="server">
                    <asp:HyperLink ID="lnkZarpe_First10HomeZarpeResponsive" runat="server" NavigateUrl="~/Zarpe/First10_Home_Zarpe.aspx">- 
                    <asp:Label ID="lbZarpe_First10HomeZarpeResponsive" runat="server" Text="Mis Primeros $10.00"></asp:Label> </asp:HyperLink></li>

                <li id="liMenuZarpe_First10SendCouponZarpeResponsive" runat="server">
                    <asp:HyperLink ID="lnkZarpe_First10SendCouponZarpeResponsive" runat="server" NavigateUrl="~/Zarpe/First10_SendCoupon_Zarpe.aspx">- 
                    <asp:Label ID="lbZarpe_First10SendCouponZarpeResponsive" runat="server" Text="Envie Descuentos a tus Amigos"></asp:Label> </asp:HyperLink></li>

                <%--<li><asp:HyperLink ID="HyperLink17" runat="server" NavigateUrl="~/Zarpe/Get3_Home_Zarpe.aspx">- 
                    <asp:Label ID="Label35" runat="server" Text="Consiga 3, reciba el suyo GRATIS"></asp:Label> </asp:HyperLink></li>
                <li><asp:HyperLink ID="HyperLink18" runat="server" NavigateUrl="~/Zarpe/Dashboard_Zarpe.aspx">- 
                    <asp:Label ID="Label40" runat="server" Text="Tablero de Control"></asp:Label> </asp:HyperLink></li>--%>
                </ul>
            </li>


            <li role="presentation" class="nav-mov" data-nav="rutina" id="liMenuPurchaseResponsive" runat="server">
                <div class="btn_comprar" >
                 <asp:HyperLink ID="lnkPurchaseResponsive" runat="server" NavigateUrl="~/Modules/Sales/ShoppingCar_02_Products.aspx">
                    <asp:Label ID="lbPurchaseResponsive" runat="server" Text="Comprar" ForeColor="#ffffff"></asp:Label>
                 </asp:HyperLink>
                 </div>
            </li>

            <li role="presentation" class="nav-mov" data-nav="plan365" id="liMenuPlan365Responsive" runat="server" visible="false">
                <asp:HyperLink ID="lnkPlan365Responsive" runat="server" NavigateUrl="~/Modules/Sales/ShoppingCar_01_Home.aspx">
                        <asp:Label ID="lbPlan365Responsive" runat="server" Text="Plan 365"></asp:Label>
                 </asp:HyperLink>  
            </li>
        </ul>
        <div class="" style="margin-top:30px; margin-left:20px;">
            <small>
                <asp:Image ID="imgMailBlack" runat="server" ImageUrl="~/Styles/images/icono_mail_black.png" alt="" Width="30px" /> 
                <asp:Label ID="lbMailBlack" runat="server" Text="Email: info@ganolife.com"> </asp:Label>
            </small>
        </div>
    </div>

</div>

<asp:UpdatePanel ID="upMasterPage" runat="server">
<ContentTemplate>



<!-- Menu Superior -->
    <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" background:#042743!important;" id="divHiddenInShare" runat="server">
    <tr>
    <td align="center"> 

    <table width="96%" border="0" align="center" cellpadding="0" cellspacing="0" style="max-width:1100px">
        <tr>
        <td>
            <ul class="nav navbar-nav--top ">
                <!-- Menu Movil -->
                <li class="dropdown">
                    
                    


                    
                    <asp:HyperLink ID="HyperLink5" runat="server"  href="#" class="dropdown-toggle ver_en_movil" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                        <div class="ver_en_movil" >
                        <asp:Image ID="imgMenuLogin" runat="server" ImageUrl="~/Styles/images/zarpe_menu1.jpg" class="zarpe_iconomenu"/>
                        <asp:Label ID="Label60" runat="server" ForeColor="#ffffff" Text="MENÚ" class="texto_18" style="margin-left:10px;" ></asp:Label>
                        </div>
                    </asp:HyperLink>
                    

                    <ul class="dropdown-menu dropdown-menu--black" style="width:100px!important;margin-left:10px!important; min-width:170px!important;">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink7" runat="server" Text="IR A GANOLIFE.COM" style="display:none;" 
                        NavigateUrl="https://www.ganolife.com" Target="_blank" Font-Bold="true" class="texto_18" ForeColor="#042842"></asp:HyperLink>
                        </li>
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink10" runat="server" Text="IR A ZAR.PE" style="display:none;" 
                        NavigateUrl="https://www.zar.pe/" Target="_blank" 
                        Font-Bold="true" class="texto_18" ForeColor="#042842"></asp:HyperLink>
                        </li>

                        
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink41" runat="server" Text="Inicio" 
                        NavigateUrl="~/Home_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink42" runat="server" Text="Fórmula" 
                        NavigateUrl="~/Secret_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink44" runat="server" Text="Súper Alimentos" 
                        NavigateUrl="~/SuperAlimentos_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink45" runat="server" Text="Productos" 
                        NavigateUrl="~/Products_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink46" runat="server" Text="Negocio en línea" 
                        NavigateUrl="~/Share_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink47" runat="server" Text="Oportunidad" 
                        NavigateUrl="~/Opportunity_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink48" runat="server" Text="Comprar" 
                        NavigateUrl="~/Modules/Sales/ShoppingCar_02_Products.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            
                            <hr style="background:#a7b0c1!important; margin: 1px!important; margin-left:15px!important; margin-bottom:12px!important;">
                       
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink49" runat="server" Text="Mi cuenta" 
                        NavigateUrl="~/Zarpe/Profile_Zarpe.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>
                            <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="lnkMenuBackOfficeResponsive" runat="server" Text="Oficina Virtual" 
                        NavigateUrl="#" Target="_blank" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>


                         <hr style="background:#a7b0c1!important; margin: 3px!important; margin-left:15px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink51" runat="server" Text="Contacto" 
                        NavigateUrl="~/ContactUs.aspx" Font-Bold="true" class="texto_20" ForeColor="#042745"></asp:HyperLink>
                        </li>

                    </ul>
                </li> 


                <!-- Link Oficina vitual -->
                <li>
                    <asp:HyperLink ID="lnkMenuBackOffice" runat="server" NavigateUrl="#" Target="_blank" CssClass="no_ver_en_movil4">
                    <asp:Label ID="Label55" runat="server" ForeColor="#ffffff" Text="OFICINA VIRTUAL" class="texto_18"></asp:Label>
                    <asp:Image ID="Image27" runat="server" ImageUrl="~/Styles/images/icono_persona1.png" Width="23px" style="margin-top:-3px;"/>
                    </asp:HyperLink>
                </li>

                

            </ul>
        </td>


        <td align="right"> 
            
                    <ul class="nav navbar-nav--top">

                    <!-- Idioma -->
                    <ul id="Ul1" class="nav navbar-nav navbar-right navbar-nav--top" runat="server" visible="false">
                        <li class="dropdown">
                                    <asp:HyperLink ID="lnkSelectLanguage" runat="server" href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                                    <asp:Label ID="Label26" runat="server" ForeColor="#ffffff" Text="English"></asp:Label> <span style="color: #ffffff" class="caret"></span>
                                    </asp:HyperLink>
                            <ul class="dropdown-menu dropdown-menu--black menu-country" style="padding:0px!important;">
                                <li>
                                    <asp:HyperLink ID="lnkLanguageSpanish" runat="server"  href="#">
                                    <asp:Label ID="lbLanguageSpanish" runat="server" Text="ESPAÑOL"></asp:Label>
                                    </asp:HyperLink> 
                                </li>
                                <li style="margin-top:-8px;">
                                    <asp:HyperLink ID="lnkLanguageEnglish" runat="server"  href="#">
                                    <asp:Label ID="lbLanguageEnglish" runat="server" Text="INGLES"></asp:Label>
                                    </asp:HyperLink> 
                                </li>
                            </ul>
                        </li>
                    </ul>


<%--                        <li id="Li2" style="display:none;" runat="server" visible="false">
                            <asp:HyperLink ID="lnkMenuBackOffice" runat="server" NavigateUrl="http://www.myganolife.com/Login.aspx" Target="_blank">
                            <asp:Label ID="lbMenuBackOffice" runat="server" Text="Oficina Virtual " ForeColor="#ffffff" ></asp:Label>
                            <asp:Image ID="imgMenuBackOffice" runat="server" ImageUrl="~/Styles/images/icono_oficina.png" />
                            </asp:HyperLink>
                        </li>--%>




                <!-- Mi cuenta -->
                <li class="dropdown" id="liMenuAccount" runat="server">
                    <asp:HyperLink ID="lnkMenuAccount" runat="server"  href="#" class="dropdown-toggle texto_18 no_ver_en_movil2" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                        <asp:Label ID="lbMenuAccount" runat="server" ForeColor="#ffffff" Text="MI CUENTA "></asp:Label>
                        <%--<span style="color: #ffffff" class="caret"></span>--%>
                        <asp:Image ID="Image9" runat="server" ImageUrl="~/Styles/images/flecha_abajo.jpg" Width="15px" style="margin-top:-5px;"/>
                    </asp:HyperLink>
                    <ul class="dropdown-menu dropdown-menu--black" style="margin-top: 9px!important; ">
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="lnkAccountProfile" runat="server" Text="MI PERFIL" Font-Bold="true" class="texto_18" ForeColor="#042842" NavigateUrl="~/Zarpe/Profile_Zarpe.aspx" ></asp:HyperLink></li>
<%--								<li><asp:HyperLink ID="lnkAccountOrders" runat="server" Text="Administrar Ordenes" NavigateUrl="~/Modules/Account/Orders.aspx#top" ></asp:HyperLink></li>
                        <li><asp:HyperLink ID="lnkCanceled" runat="server" Text="Cancelar Ordenes" NavigateUrl="~/Modules/Account/Canceled.aspx#top" ></asp:HyperLink></li>--%>
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="lnkAddress" runat="server" Text="Configurar Direcciones" Font-Bold="true" class="texto_18" ForeColor="#042842" NavigateUrl="~/Modules/Account/Address.aspx#top" Visible="false"></asp:HyperLink></li>
                        <li class="zarpe_margen_izquierda4"><asp:HyperLink ID="HyperLink6" runat="server" Text="Compartir" Font-Bold="true" class="texto_18" ForeColor="#042842" NavigateUrl="~/Modules/Account/Share.aspx#top" Visible="false"></asp:HyperLink></li>
                    </ul>
                </li>


                <!-- Nombre -->
                <li>
                    <asp:LinkButton ID="lnkMenuLogin" runat="server" OnClick="lnkMenuLogin_Click" >
                    <asp:Label ID="lbLoginName" ForeColor="#ffffff" runat="server" class="texto_19"></asp:Label>
                    <asp:Label ID="lbLoginStatus" ForeColor="#ffffff" runat="server" class="texto_19"></asp:Label>
    <%--                            <asp:Image ID="imgMenuLogin" runat="server" ImageUrl="~/Styles/images/icono_ingresar_l.jpg" />--%>
                    </asp:LinkButton>
                </li>






                        <!-- Carrito -->
                        <li class="dropdown ">
                            <asp:HyperLink ID="lnkShopingCart" runat="server"  href="#" class="dropdown-toggle " data-toggle="dropdown" role="button" 
                            aria-haspopup="true" aria-expanded="false" style="margin-top:0px;">

                            <asp:Label ID="Label23" runat="server" ForeColor="#ffffff" Text="CARRITO" CssClass="no_ver_en_movil4 texto_18"></asp:Label>
                                 <div class="ancho_carrito_boton" >
                                 <asp:Image ID="imgShopingCart" runat="server" ImageUrl="~/Styles/images/icono_carrito3.gif" class="ancho_icono_carrito" 
                                 style="margin-top:-3px;"/>
                                 <div style="color:#042842; height:15px;text-align:center; width:30px;
                                     display: inline-block; margin-top:1px; margin-right:-3px; margin-left: -10px;">
                                    <asp:Label ID="lbQtyItems" runat="server" Text="0" CssClass="texto_7" style="margin-top:0px;"></asp:Label>
                                </div>
                                </div> 
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black dropdown-menu--cart menu_carrito" id="ulDivShoppingCar" 
                            style="background:#ffffff!important;" runat="server">
                            <div ID="divShoppingCar_1" runat="server" style="text-align: center">
                                <div class="img">
                                    <asp:Image ID="imgShoppingCarEmpty" runat="server" ImageUrl="~/Styles/images/icono_compras_c.png" style=" width:60%; max-width:90px;" />
                                </div>
                                <p><asp:Label ID="Label11" runat="server" Text="Su carrito de compras está vacio" class="texto_18"></asp:Label></p>
                     
                                 <%--<asp:LinkButton ID="lnkShoppingCarEmpty" runat="server" class="btn btn-success btn-ganolife2" Text="COMPRAR AHORA" onclick="lnkShoppingCarEmpty_Click"></asp:LinkButton>--%>
                            </div>

                            <div ID="divShoppingCar_2" runat="server" >
                                <asp:Label ID="Label4" runat="server" Text="Últimos items agregados" class="texto_7" ForeColor="#58595B"></asp:Label>                   
                                <br><br>

                                <table width="100%">

                                <asp:DataList ID="dtlMasterOrderLines" runat="server"
                                ClientIDMode="Static" TabIndex="86" RepeatDirection="Horizontal" RepeatLayout="Flow"
                                onitemdatabound="dtlMasterOrderLines_ItemDataBound">
                                    <ItemTemplate>

                                    <table width="94%" border="0" align="center" cellpadding="0" cellspacing="0" 
                                    style=" text-align:right !important;">
                                      <tr>
                                        <td style="background-color:#ffffff;text-align: left;">
                                        <asp:Image ID="imgItemProduct" runat="server" 
                                        ImageUrl='<%# "~/Styles/images/Products/zarpe/"+DataBinder.Eval(Container.DataItem, "ProductID")+"_zarpe_producto_2.jpg" %>' 
                                        width="50px"/></td>
                                        <td><asp:Label ID="lbItemProductName" runat="server" 
                                        Text='<%# DataBinder.Eval(Container.DataItem, "ProductName") %>' CssClass="texto_7"  ForeColor="#58595B"></asp:Label></td>
                                        <td><asp:Label ID="lbItemPrice" runat="server" 
                                        Text='<%# DataBinder.Eval(Container.DataItem, "WholesalePrice", "{0:###,##0.00} USD") %>' 
                                        CssClass="texto_7" Font-Bold="true" ForeColor="#333333"></asp:Label></td>
                                      </tr>
                                      <tr>
                                        <td colspan="3"><hr style="background:#a7a8ac!important; margin-top: 2px!important; 
                                                            margin-bottom: 6px!important;"></td>
                                      </tr>
                                    </table>

                                    </ItemTemplate>
                                </asp:DataList>

                                <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" text-align:right !important;">
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblShipCost" runat="server" Text="Envío" CssClass="texto_7" ForeColor="#58595B"></asp:Label>
                                    </td>
	                                <td style="width:30%">
                                        <asp:Label ID="lbShipCost" runat="server" Font-Bold="true" CssClass="texto_7" ForeColor="#333333"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblSubTotal" runat="server" Text="Subtotal" CssClass="texto_7" ForeColor="#58595B"></asp:Label>
                                    </td>
	                                <td style="width:30%">
                                        <asp:Label ID="lbSubTotal" runat="server" Font-Bold="true" CssClass="texto_7" ForeColor="#333333"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblTaxAmt" runat="server" Text="Impuesto" CssClass="texto_7" ForeColor="#58595B"></asp:Label>
                                    </td>
	                                <td style="width:30%">
                                        <asp:Label ID="lbTaxAmt" runat="server" Font-Bold="true" CssClass="texto_7" ForeColor="#333333"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblTotal" runat="server" Text="Total" CssClass="texto_7" ForeColor="#58595B"></asp:Label>
                                    </td>
	                                <td style="width:30%">
                                        <asp:Label ID="lbTotal" runat="server" Font-Bold="true" CssClass="texto_7" ForeColor="#333333"></asp:Label>
                                    </td>
                                </tr>
                                </table>
                                <br>

								<div style="text-align:right">
                                    <asp:LinkButton ID="lnkShoppingCar_Resume" runat="server" class="boton_celeste4" ForeColor="#001E3A" 
                                    Font-Bold="true" style="margin:0px!important;" OnClick="lnkShoppingCar_Resume_Click">
                                    <asp:Label ID="Label5" runat="server" Text="Ver carrito"></asp:Label>
                                    </asp:LinkButton><br><br>
									<asp:LinkButton ID="lnkShoppingCar_02" runat="server" class="boton_celeste4" ForeColor="#001E3A" 
                                    Font-Bold="true" style="margin:0px!important; margin-right: -4px!important;" OnClick="lnkShoppingCar_02_Click" >
                                    <asp:Label ID="Label6" runat="server" Text="Realizar Pago"></asp:Label>
                                    </asp:LinkButton>
                                    <br><br>
								</div>

                            </div>

                            </ul>
                        </li>

                        <%-- LAST ITEM --%>
                        <li class="dropdown">
                            <asp:HyperLink ID="lnkShopingCartLastItem" runat="server"  href="#" class="dropdown-toggle"
                             data-toggle="dropdown" role="button"  visible="true"
                            aria-haspopup="true" aria-expanded="false" style="margin-top:-26px; margin-left: -30px; ">
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black dropdown-menu--cart menu_carrito zarpe_margen_izquierda5" 
                            style="margin-top:18px; width:200px!important; background:#ffffff!important; padding:10px; "
                            id="ulDivShoppingCarLastItem" runat="server">

                           <%-- <div ID="ulDivShoppingCarLastItem" runat="server" style=""></div>--%>

                            <div ID="divShoppingCar_LastItem" runat="server" style=" line-height:1;">
                                <asp:Label ID="Label18" runat="server" Text="Últimos items agregados" class="texto_7" ForeColor="#58595B"></asp:Label>
                                <br><br>
                                <asp:DataList ID="dtlMasterOrderLinesLastItem" runat="server"
                                ClientIDMode="Static" TabIndex="86" RepeatDirection="Horizontal" RepeatLayout="Flow"
                                onitemdatabound="dtlMasterOrderLines_ItemDataBound">
                                    <ItemTemplate>

                                    <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" text-align:right !important;">
                                      <tr>
                                        <td style="background-color:#ffffff;text-align: center;">
                                        <asp:Image ID="imgItemProduct" runat="server" 
                                        ImageUrl='<%# "~/Styles/images/Products/zarpe/"+DataBinder.Eval(Container.DataItem, "ProductID")+"_zarpe_producto_2.jpg" %>' 
                                        width="50px" /></td>
                                        <td><asp:Label ID="lbItemProductName" runat="server" 
                                        Text='<%# DataBinder.Eval(Container.DataItem, "ProductName") %>' CssClass="texto_7"  ForeColor="#58595B" ></asp:Label></td>
                                        <td><asp:Label ID="lbItemPrice" runat="server" 
                                        Text='<%# DataBinder.Eval(Container.DataItem, "WholesalePrice", "{0:###,##0.00} USD") %>' 
                                        CssClass="texto_7" Font-Bold="true" ForeColor="#333333"></asp:Label></td>
                                      </tr>
                                      <tr>
                                        <td colspan="3"><br>
                                        <hr style="background:#a7a8ac!important;  margin-top: 2px!important; margin-bottom: 6px!important;">
                                        </td>
                                      </tr>
                                    </table>

                                    </ItemTemplate>
                                </asp:DataList>
                                <br>
                                
                                    <asp:Label ID="lbMessage_LastItem" CssClass="texto_7" ForeColor="#58595B" runat="server"></asp:Label>
                                    <br><br>
                                    <asp:LinkButton ID="lnkShoppingCar_02LastItem" runat="server"  class="boton_celeste4" ForeColor="#001E3A" 
                                    Font-Bold="true" style="margin:0px!important;"
                                    OnClick="lnkShoppingCar_02_Click">
                                    <asp:Label ID="lbShoppingCar_02LastItem" runat="server" Text="Realizar Pago"></asp:Label>
                                    </asp:LinkButton>
                                <br><br><br>
                                
                            </div>


                            </ul>
                        </li>

                        <!-- Contacto -->
                        <li>
                            <asp:HyperLink ID="lnkContanctUs" runat="server" NavigateUrl="~/ContactUs.aspx" CssClass="no_ver_en_movil4">
                            <asp:Label ID="Label28" runat="server" ForeColor="#ffffff" Text="CONTACTO" class="texto_18"></asp:Label><span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>

                        <!-- Pais -->
                        <li class="dropdown">
                            <asp:HyperLink ID="lnkSelectCurrentCountryMenu" runat="server" href="#" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                                <asp:Label ID="lblCurrentCountry" runat="server" ClientIDMode="Static" ForeColor="#ffffff" class="texto_18" Text="País"></asp:Label>
                                <asp:Image ID="imgCurrentCountry" runat="server" ClientIDMode="Static" class="zarpe_iconomenu" style=" margin-left:5px;" />
                                <asp:Image ID="Image8" runat="server" ImageUrl="~/Styles/images/flecha_abajo.jpg" Width="15px" style="margin-top:-1px;"/>
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black menu-country menu_pais" style="margin-left: -70px!important; background:#ffffff!important; width:140px; ">
                            <asp:DataList ID="dtlCountriesMenu" runat="server" ClientIDMode="Static" RepeatDirection="Horizontal" RepeatLayout="Flow">
                            <ItemTemplate>

                            <asp:HiddenField ID="hdCountryID" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryID") %>' Visible="false" />
                            <asp:HiddenField ID="hdCountryName" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' Visible="false" />

                            <li class="zarpe_margen_izquierda4">
                                <asp:Image ID="imgItemCountry" runat="server" style="margin-left:5px;" Width="22px" ImageUrl='<%# "~/Styles/images/Country/"+DataBinder.Eval(Container.DataItem, "CountryID")+".png" %>' />
                                <asp:LinkButton ID="lnkCountry" runat="server" style=" margin-left:5px;" class="texto_18" ForeColor="#042842"
                                Text='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' OnClick="lnkCountry_Click" ></asp:LinkButton>
                            </li>

                            </ItemTemplate>
                            </asp:DataList>
                            </ul>
                        </li>

                        <!-- Cerrar sesión -->
                        <li>
                        <asp:LinkButton ID="lnkMenuLogOff" runat="server" OnClick="lnkMenuLogOff_Click">
                            <asp:Image ID="imgMenuLogOff" runat="server" ImageUrl="~/Styles/images/icono_salir_blanco.png"  class="zarpe_iconomenu" />
                        </asp:LinkButton>
                        </li>


                    </ul>
        </td>
        </tr>
    </table>
       
    </td>
    </tr>
    </table>


<%--<nav ID="navMenuChanging" runat="server" class="menu_6" ></nav>--%>

<!-- Menu Secundario -->
<table align="center" border="0" cellspacing="0" cellpadding="0"  style="width:100%; max-width:2000px;" >
<tr>
<td>

<%--<nav ID="navMenuChanging222" runat="server" class="menu_7" style="display:none;" ></nav>--%>

<nav ID="navMenuChanging" runat="server" class="menu_2" >
        <div class="container-fluid container" >
            
            <div style="margin-top:30px;">

                <div class="logo_menu_1">
                    <asp:HyperLink ID="lnkHome1" runat="server" NavigateUrl="~/Home_Zarpe.aspx">
                        <asp:Image ID="Image28" runat="server" ImageUrl="~/Styles/images/logo_zarpe3.png" alt="" />
                    </asp:HyperLink>
                </div>

                <div class="logo_menu_2">
                    <asp:HyperLink ID="lnkHome2" runat="server" NavigateUrl="~/Home_Zarpe.aspx">
                        <asp:Image ID="Image29" runat="server" ImageUrl="~/Styles/images/logo_zarpe.png" alt="" />
                    </asp:HyperLink>
                </div>
                <div class="responsive " style=" display:none;">
                    <button type="button" class="navbar-toggle collapsed" href="#drawerExample" data-toggle="drawer" aria-foldedopen="false" aria-controls="drawerExample">
                        <!-- <span class="sr-only">Toggle navigation</span> -->
                        <span class="icon-bar"></span>
                        <span class="icon-bar"></span>
                        <span class="icon-bar">+
                        </span>
                    </button>
                    <div class="col-xs-1 responsive__opt">
                        <asp:HyperLink ID="lnkLogoGanolifeResponsive" runat="server" class="logo" NavigateUrl="~/Home.aspx">
                            <asp:Image ID="imgLogoGanolifeResponsive" runat="server" ImageUrl="~/Styles/images/logo-responsive-2.png" Width="28px"/>
                        </asp:HyperLink>
                    </div>


                    <div class="col-xs-offset-1 col-xs-7 responsive__opt ancho_tablet_1" style="padding-left: 0px; margin-left: 7px!important;">
                        
<%--                        <asp:HyperLink ID="lnkMenuBackOfficeResponsive" runat="server" NavigateUrl="#" Target="_blank">
                            <asp:Image ID="imgMenuBackOfficeResponsive" runat="server" ImageUrl="~/Styles/images/icono_oficina_2.png" Width="24px" />
                        </asp:HyperLink>--%>


                        <!-- Iniciar sesion -->
                        <asp:LinkButton ID="lnkMenuLoginResponsive" runat="server" OnClick="lnkMenuLogin_Click">
                            <%--<asp:Image ID="imgMenuLoginResponsive" runat="server" ImageUrl="~/Styles/images/icono_ingresar_l.png" visible="false" />--%>
                            <asp:Image ID="imgMenuLoginResponsive" runat="server" ImageUrl="~/Styles/images/icono_ingresar_gris.png" Width="24px" />
                        </asp:LinkButton>


                        <!-- Cuando Inicia sesion aparece este icono Perfil -->
                        <asp:HyperLink ID="lnkMenuProfileResponsive" runat="server" NavigateUrl="~/Zarpe/Profile_Zarpe.aspx">
                             <asp:Image ID="imgMenuProfileResponsive" runat="server" ImageUrl="~/Styles/images/profile-icon.png" alt="" />
                        </asp:HyperLink>


                        <div class="dropdown">
                            <asp:HyperLink ID="lnkShopingCartResponsive" runat="server" href="" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                                <asp:Image ID="imgShoppingCartResponsive" runat="server" ImageUrl="~/Styles/images/cart.png" alt="" />
                                <span class="badge">
                                <asp:Label ID="lbQtyItemsResponsive" runat="server" Text="0" ></asp:Label>
                                </span>
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black dropdown-menu--cart">

                            <div ID="divShoppingCar_1Responsive" runat="server">
                                <div class="img">
                                    <asp:Image ID="imgShoppingCarEmptyResponsive" runat="server" ImageUrl="~/Styles/images/icono_compras_b.png" />
                                </div>
                                <p><asp:Label ID="Label2" runat="server" Text="Su carrito de compras está vacio" ></asp:Label></p>
                               <hr />
                                 <%--<asp:LinkButton ID="lnkShoppingCarEmptyResponsive" runat="server" class="btn btn-success btn-ganolife" Text="COMPRAR AHORA" onclick="lnkShoppingCarEmpty_Click"></asp:LinkButton>--%>
                            </div>

                            <div ID="divShoppingCar_2Responsive" runat="server">
                                <asp:Label ID="Label1" runat="server" Text="Últimos items agregados" class="texto_7" ForeColor="#58595B"></asp:Label>
                                <br><br>
                                <asp:DataList ID="dtlMasterOrderLinesResponsive" runat="server"
                                ClientIDMode="Static" TabIndex="86" RepeatDirection="Horizontal" RepeatLayout="Flow"
                                onitemdatabound="dtlMasterOrderLines_ItemDataBound">
                                    <ItemTemplate>
                                    <table width="90%" border="0" align="center" cellpadding="0" cellspacing="0" style=" text-align:right !important;">
                                    <tr >
                                        <td style="background-color:#ffffff;text-align: left;">
                                            <asp:Image ID="imgItemProduct" runat="server" 
                                            ImageUrl='<%# "~/Styles/images/Products/zarpe/"+DataBinder.Eval(Container.DataItem, "ProductID")+"_zarpe_producto_2.jpg" %>' 
                                            width="50px" />
                                        </td>
                                        <td align="left">
                                             <asp:Label ID="lbItemProductName" runat="server" Text='<%# DataBinder.Eval(Container.DataItem, "ProductName") %>' 
                                             CssClass="texto_7"  ForeColor="#58595B"></asp:Label>
                                        </td>
                                        <td>
                                            <asp:Label ID="lbItemPrice" runat="server" 
                                            Text='<%# DataBinder.Eval(Container.DataItem, "WholesalePrice", "{0:###,##0.00} USD") %>' 
                                            CssClass="texto_7" Font-Bold="true" ForeColor="#333333"></asp:Label>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td colspan="3">
                                        <hr style="background:#a7a8ac!important;  margin-top: 2px!important; margin-bottom: 6px!important;">
                                        </td>
                                    </tr>
                                    </table>
                                    </ItemTemplate>
                                </asp:DataList>

                                <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" text-align:right !important;">
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblShipCostResponsive" runat="server" CssClass="texto_7" ForeColor="#58595B" Text="Envío"></asp:Label>
                                    </td>
	                                <td style="width:40%">
                                        <asp:Label ID="lbShipCostResponsive" runat="server" CssClass="texto_7" Font-Bold="true" ForeColor="#58595B"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblSubTotalResponsive" runat="server" CssClass="texto_7" ForeColor="#58595B" Text="Subtotal"></asp:Label>
                                    </td>
	                                <td style="width:40%">
                                        <asp:Label ID="lbSubTotalResponsive" runat="server" CssClass="texto_7" Font-Bold="true" ForeColor="#58595B"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblTaxAmtResponsive" runat="server" CssClass="texto_7" ForeColor="#58595B" Text="Impuesto"></asp:Label>
                                    </td>
	                                <td style="width:40%">
                                        <asp:Label ID="lbTaxAmtResponsive" runat="server" CssClass="texto_7" Font-Bold="true" ForeColor="#58595B"></asp:Label>
                                    </td>
                                </tr>
                                <tr class="list-inline cart-subtotals text-right">
                                    <td style="width:30%"></td>
	                                <td >
                                        <asp:Label ID="lblTotalResponsive" runat="server" CssClass="texto_7" ForeColor="#58595B" Text="Total"></asp:Label>
                                    </td>
	                                <td style="width:40%">
                                        <asp:Label ID="lbTotalResponsive" runat="server" CssClass="texto_7" Font-Bold="true" ForeColor="#58595B"></asp:Label>
                                    </td>
                                </tr>
                                </table>

                                <br>

								<div class="cart-buttons ">
                                    <asp:LinkButton ID="lnkShoppingCar_ResumeResponsive" runat="server" class="boton_celeste4" ForeColor="#001E3A" 
                                    Font-Bold="true" style="margin:0px!important;" OnClick="lnkShoppingCar_Resume_Click" >
                                    <asp:Label ID="lblShoppingCar_Resume" runat="server" Text="Ver carrito"></asp:Label>
                                    </asp:LinkButton><br><br>
									<asp:LinkButton ID="lnkShoppingCar_02Responsive" runat="server" class="boton_celeste4" ForeColor="#001E3A" 
                                    Font-Bold="true" style="margin:0px!important;" OnClick="lnkShoppingCar_02_Click">
                                    <asp:Label ID="lblShoppingCar_02Reponsive" runat="server" Text="Realizar Pago"></asp:Label>
                                    </asp:LinkButton>
								</div>

							</div>

                            </ul>
                        </div>

   

                        <!-- Idiomas tablet -->
                        <div id="Div1" class="dropdown" runat="server" visible="false">
                            <asp:HyperLink ID="HyperLink1" runat="server" href="" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                                <asp:Image ID="Image7" runat="server" ImageUrl="~/Styles/images/idiomas.png" alt="" />
                            </asp:HyperLink>
                            <ul class="dropdown-menu dropdown-menu--black menu-country" style="padding:20px!important;">
                                <li>
                                    <asp:HyperLink ID="HyperLink3" runat="server"  href="#">
                                    <asp:Label ID="Label10" runat="server" Text="ESPAÑOL"></asp:Label>
                                    </asp:HyperLink> 
                                </li>
                                <li>
                                    <asp:HyperLink ID="HyperLink4" runat="server"  href="#">
                                    <asp:Label ID="Label12" runat="server" Text="INGLES"></asp:Label>
                                    </asp:HyperLink> 
                                </li>
                            </ul>
                        </div>



                        <!-- Paises tablet -->
                        <div class="dropdown">
                            <asp:HyperLink ID="lnkSelectCurrentCountryMenuResponsive" runat="server" href="" class="dropdown-toggle" data-toggle="dropdown" role="button" 
                            aria-haspopup="true" aria-expanded="false">
                            <asp:Image ID="imgCurrentCountryResponsive" runat="server" Width="24px" ImageUrl="~/Styles/images/paises.png" alt="" />
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black menu-country">
                            <asp:DataList ID="dtlCountriesMenuPopup" runat="server" ClientIDMode="Static" RepeatDirection="Horizontal" RepeatLayout="Flow">
                            <ItemTemplate>

                            <asp:HiddenField ID="hdCountryID" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryID") %>' Visible="false" />
                            <asp:HiddenField ID="hdCountryName" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' Visible="false" />

                            <li>
                                <asp:Image ID="imgItemCountry" runat="server" style="margin-left:8px;" Width="22px" ImageUrl='<%# "~/Styles/images/Country/"+DataBinder.Eval(Container.DataItem, "CountryID")+".png" %>' />
                                <asp:LinkButton ID="lnkCountry" runat="server" style=" margin-left:8px;" Text='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' OnClick="lnkCountry_Click" ></asp:LinkButton>
                            </li>

                            </ItemTemplate>
                            </asp:DataList>
                            </ul>
                        </div>



                        <!-- Cerrar sesion -->
                        <asp:LinkButton ID="lnkMenuLogOffResponsive" runat="server" OnClick="lnkMenuLogOff_Click">
                            <asp:Image ID="imgMenuLogOffResponsive" runat="server" ImageUrl="~/Styles/images/icono_salir_gris.png" Width="24px"  />
                        </asp:LinkButton>

                        <%-- LAST ITEM RESPONSIVE --%>
                        <div class="dropdown">
                            <asp:HyperLink ID="lnkShopingCartLastItemResponsive" runat="server" href="" class="dropdown-toggle"  Visible="true" 
                            data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                            </asp:HyperLink>

                            <ul class="dropdown-menu dropdown-menu--black dropdown-menu--cart" id="ulDivShoppingCarLastItemResponsive" runat="server">
                            <div ID="divShoppingCar_LastItemResponsive" runat="server">
                                <strong><asp:Label ID="Label21" runat="server" Text="Últimos items agregados"></asp:Label></strong>
                                <br />
                                
                                    <asp:DataList ID="dtlMasterOrderLinesLastItemResponsive" runat="server"
                                    ClientIDMode="Static" TabIndex="86" RepeatDirection="Horizontal" RepeatLayout="Flow"
                                    onitemdatabound="dtlMasterOrderLines_ItemDataBound">
                                    <ItemTemplate>
                                    <table width="90%" border="0" align="center" cellpadding="0" cellspacing="0" style=" text-align:right !important;">
                                    <tr>
                                        <td style="background-color:#ffffff;text-align: left;">
                                            <asp:Image ID="imgItemProduct" runat="server" ImageUrl='<%# "~/Styles/images/Products/zarpe/"+DataBinder.Eval(Container.DataItem, "ProductID")+"_zarpe_producto_2.jpg" %>' width="60px" />
                                        </td>
                                        <td align="left">
                                             <asp:Label ID="lbItemProductName" runat="server" Text='<%# DataBinder.Eval(Container.DataItem, "ProductName") %>' 
                                             CssClass="menu_carrito_texto1" ForeColor="#333333"></asp:Label>
                                        </td>
                                        <td>
                                            <asp:Label ID="lbItemPrice" runat="server" Text='<%# DataBinder.Eval(Container.DataItem, "WholesalePrice", "{0:###,##0.00} USD") %>' CssClass="menu_carrito_texto1" ForeColor="#333333"></asp:Label>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td colspan="3"><hr style=" border-color:#AFAFAF !important;"></td>
                                    </tr>
                                    </table>
                                    </ItemTemplate>
                                </asp:DataList>
                                
                                <br>
                                <asp:Label ID="lbMessage_LastItemResponsive" runat="server"></asp:Label>
                                <br />
                                <asp:LinkButton ID="lnkShoppingCar_02LastItemResponsive" runat="server" class="btn btn-success btn-ganolife" OnClick="lnkShoppingCar_02_Click">
                                <asp:Label ID="lbShoppingCar_02LastItemResponsive" runat="server" Text="Realizar Pago"></asp:Label>
                                </asp:LinkButton>
                 
							</div>
                            </ul>
                        </div>

                    </div>
                </div>
            </div>

            <!-- Menu Principal -->
            <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1"  style=" margin-top:-74px;">
                
                <div class="clear"></div>
                <div class="wrapper wrapper--fixed">
                    <ul class="nav navbar-nav navbar-right navbar-nav--bottom zarpe_pc">
                        <li class="nav-mov" id="liMenuHome" runat="server">
                            <asp:HyperLink ID="lnkHome" runat="server" NavigateUrl="~/Home_Zarpe.aspx">
                                <asp:Label ID="lbHome" runat="server" Text="Inicio"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <li class="nav-mov" id="liMenuSecret" runat="server">
                            <asp:HyperLink ID="lnkSecret" runat="server" NavigateUrl="~/Secret_Zarpe.aspx">
                            <asp:Label ID="lbSecret" runat="server" Text="Fórmula"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <li class="nav-mov" id="liMenuSuper" runat="server">
                            <asp:HyperLink ID="lnkSuper" runat="server" NavigateUrl="~/SuperAlimentos_Zarpe.aspx">
                            <asp:Label ID="lbSuper" runat="server" Text="Súper Alimentos"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <li class="nav-mov" id="liMenuProducts" runat="server">
                            <asp:HyperLink ID="lnkProducts" runat="server" NavigateUrl="~/Products_Zarpe.aspx">
                            <asp:Label ID="lbProducts" runat="server" Text="Productos"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <li class="nav-mov" id="li3" runat="server">
                            <asp:HyperLink ID="HyperLink37" runat="server" NavigateUrl="~/Share_Zarpe.aspx">
                            <asp:Label ID="Label54" runat="server" Text="Negocio en línea"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <%--<li class="nav-mov" data-nav="formula" id="liMenuFormule" runat="server">
                            <asp:HyperLink ID="lnkFormule" runat="server" NavigateUrl="~/Home.aspx#formula">
                            <asp:Label ID="lbFormule" runat="server" Text="Fórmula"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                        <li class="nav-mov" data-nav="historia" id="liMenuHistory" runat="server">
                            <asp:HyperLink ID="lnkHistory" runat="server" NavigateUrl="~/Home.aspx#historia">
                            <asp:Label ID="lbHistory" runat="server" Text="Historia"></asp:Label> <span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>--%>
                        
                        <%--<li class="nav-mov" >
                            <asp:HyperLink ID="HyperLink5" runat="server" NavigateUrl="http://get.ganolife.com/plan2016/" target="_blank">
                            <asp:Label ID="Label14" runat="server" Text="Oportunidad"></asp:Label> 
                            </asp:HyperLink>
                        </li>--%>

                        <li class="nav-mov" id="liMenuOportunity" runat="server">
                            <asp:HyperLink ID="lnkOportunity" runat="server" NavigateUrl="~/Opportunity_Zarpe.aspx">
                            <asp:Label ID="lbOportunity" runat="server" Text="Oportunidad"></asp:Label> 
                            </asp:HyperLink>
                        </li>

                        <li class="nav-mov"  style=" display:none;">
                            <div ID="HyperLink9" runat="server" href="#" data-toggle="dropdown" style="margin-top:13px; padding-left:20px; 
                                padding-right:20px;  display:none;">
                                <asp:Label ID="Label16" runat="server" ClientIDMode="Static" ForeColor="#999999" Text="Zarpe"></asp:Label>
                            </div>

                            <ul class="dropdown-menu dropdown-menu--black menu-country" style="margin-top:16px;">

                            <li id="liMenuZarpe_HomeZarpe" runat="server">
                                <asp:HyperLink ID="lnkZarpe_HomeZarpe" runat="server" NavigateUrl="~/Zarpe/Home_Zarpe.aspx">
                                <asp:Label ID="lbZarpe_HomeZarpe" runat="server" Text="Home"></asp:Label> </asp:HyperLink></li>

                            <li id="liMenuZarpe_DashboardZarpe" runat="server">
                                <asp:HyperLink ID="lnkZarpe_DashboardZarpe" runat="server" NavigateUrl="~/Zarpe/Dashboard_Zarpe.aspx">
                                <asp:Label ID="lbZarpe_DashboardZarpe" runat="server" Text="Tablero de Control"></asp:Label> </asp:HyperLink></li>

                            <li id="liMenuZarpe_ProfileZarpe" runat="server">
                                <asp:HyperLink ID="lnkZarpe_ProfileZarpe" runat="server" NavigateUrl="~/Zarpe/Profile_Zarpe.aspx">
                                <asp:Label ID="lbZarpe_ProfileZarpe" runat="server" Text="Influenciador"></asp:Label> </asp:HyperLink></li>

                            <li id="liMenuZarpe_First10HomeZarpe" runat="server">
                                <asp:HyperLink ID="lnkZarpe_First10HomeZarpe" runat="server" NavigateUrl="~/Zarpe/First10_Home_Zarpe.aspx">
                                <asp:Label ID="lbZarpe_First10HomeZarpe" runat="server" Text="Mis Primeros $10.00"></asp:Label> </asp:HyperLink></li>

                            <li id="liMenuZarpe_First10SendCouponZarpe" runat="server">
                                <asp:HyperLink ID="lnkZarpe_First10SendCouponZarpe" runat="server" NavigateUrl="~/Zarpe/First10_SendCoupon_Zarpe.aspx">
                                <asp:Label ID="lbZarpe_First10SendCouponZarpe" runat="server" Text="Envie Descuentos a tus Amigos"></asp:Label> </asp:HyperLink></li>

                            <%--<li><asp:HyperLink ID="HyperLink12" runat="server" NavigateUrl="~/Zarpe/Get3_Home_Zarpe.aspx">
                                <asp:Label ID="Label20" runat="server" Text="Consiga 3, reciba el suyo GRATIS"></asp:Label> </asp:HyperLink></li>
                            <li><asp:HyperLink ID="HyperLink8" runat="server" NavigateUrl="~/Zarpe/Dashboard_Zarpe.aspx">
                                <asp:Label ID="Label15" runat="server" Text="Tablero de Control"></asp:Label> </asp:HyperLink></li>--%>
                            </ul>
                        </li>

                        <li class="nav-mov" id="liMenuPurchase" runat="server" >
                            <asp:HyperLink ID="lnkPurchase" runat="server" NavigateUrl="~/Modules/Sales/ShoppingCar_02_Products.aspx">
                            <asp:Label ID="lbPurchase" runat="server" Text="Comprar" Font-Bold="true"></asp:Label> 
                            </asp:HyperLink>           
                        </li>
                        <li class="nav-mov" data-nav="plan365" id="liMenuPlan365" runat="server" visible="false">
                            <asp:HyperLink ID="lnkPlan365" runat="server" NavigateUrl="~/Home.aspx#plan365">
                            <asp:Label ID="lbPlan365" runat="server" Text="Plan 365 "></asp:Label><span class="sr-only">(current)</span>
                            </asp:HyperLink>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- /.navbar-collapse -->


            <div class="boton_transparente" >
            <asp:HyperLink ID="HyperLink40" NavigateUrl="~/Opportunity_Zarpe.aspx" runat="server">
            <asp:Label ID="Label56" runat="server" Text="¡Arme su tripulación!" class="texto_3" ForeColor="#ffffff"></asp:Label>
            </asp:HyperLink> 
            
            </div>
        </div>   
</nav>

</td>
</tr>
</table>




<!-- Menu Movil Iconos / No va -->
<div style=" background:#e7e8ec!important; width:100%; display:none;" >
<article id="slider" style=" background:#e7e8ec;">
<input checked type='radio' name='slider' id='slide1' style="display:none;"/>
<input type='radio' name='slider' id='slide2' style="display:none;"/>
<%--<input type='radio' name='slider' id='slide3'/>
<input type='radio' name='slider' id='slide4'/>
<input type='radio' name='slider' id='slide5'/>--%>
<div id="slides">
	<div id="container">
		<div class="inner">
			<article>
			<asp:HyperLink ID="HyperLink18" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#videos"  runat="server">
            <asp:Image ID="Image2" runat="server" ImageUrl="~/Styles/images/zarpe_menu_1.jpg" style="width:100%; max-width:60px;" />
            <asp:Label ID="Label31" runat="server" Text="COMPARTIR VIDEOS"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink> 

            <asp:HyperLink ID="HyperLink19" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#productos" runat="server">
            <asp:Image ID="Image3" runat="server" ImageUrl="~/Styles/images/zarpe_menu_2.jpg" style="width:100%; max-width:60px;" /> 
            <asp:Label ID="Label32" runat="server" Text="COMPARTIR PRODUCTOS"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink>

            <asp:HyperLink ID="HyperLink20" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
            <asp:Image ID="Image17" runat="server" ImageUrl="~/Styles/images/zarpe_menu_3.jpg" style="width:100%; max-width:60px;" /> 
            <asp:Label ID="Label33" runat="server" Text="COMPARTIR SÚPER ALIMENTOS"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink> 

            <asp:HyperLink ID="HyperLink21" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#herramientas" runat="server">
            <asp:Image ID="Image18" runat="server" ImageUrl="~/Styles/images/zarpe_menu_4.jpg" style="width:100%; max-width:60px;" /> 
            <asp:Label ID="Label35" runat="server" Text="COMPARTIR DOCUMENTOS"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
			</article>

			<article>
            <asp:HyperLink ID="HyperLink22" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#blog" runat="server">
            <asp:Image ID="Image19" runat="server" ImageUrl="~/Styles/images/zarpe_menu_5.jpg" style="width:100%; max-width:60px;" />
            <asp:Label ID="Label36" runat="server" Text="COMPARTIR BLOG"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink>

			<asp:HyperLink ID="HyperLink23" class="menu_padding2" NavigateUrl="~/Share_Zarpe.aspx#prospectos" runat="server">
            <asp:Image ID="Image20" runat="server" ImageUrl="~/Styles/images/zarpe_menu_6.jpg" style="width:100%; max-width:60px;" />
            <asp:Label ID="Label37" runat="server" Text="CONTROL DE PROSPECTOS"  CssClass="texto_20" Font-Bold="true"></asp:Label>
            </asp:HyperLink> 
			</article>
		</div>
	</div>
</div>
<div id="commands">
	<label for='slide1'></label>
	<label for='slide2'></label>
	<%--<label for='slide3'></label>
	<label for='slide4'></label>
	<label for='slide5'></label>--%>
</div>
<div id="active" >
	<label for='slide1'></label>
	<label for='slide2'></label>
	<%--<label for='slide3'></label>
	<label for='slide4'></label>
	<label for='slide5'></label>--%>
</div>
</article>
</div>





<!-- Slider Menu Movil Iconos -->
<table id="menuShare_Movil" runat="server" width="100%" border="0" align="center" cellpadding="0" cellspacing="0" 
style="height:120px; margin-bottom:20px; background:#e6e6e6; " class="zarpe_movil">
    <tr>
    <td align="center" >
        

        <!-- Bienvenido / Share --> 
            <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" background:#ffffff!important; ">
                <tr>
                <td>
                <table width="92%" border="0" align="center" cellpadding="0" cellspacing="0" >
                <tr>
                <td align="right">
                <asp:Image ID="Image37" runat="server" ImageUrl="~/Styles/images/zarpe_logo2.jpg" style="width:120px; margin-right:20px;" />
                </td>
                <td align="right" style="line-height:0; ">
                <br>
                <asp:Label ID="Label74" runat="server" Text="Bienvenido (a)" class="titulo_8b" ForeColor="#042743" ></asp:Label>
                <asp:Label ID="Label75" runat="server" Text="Nombre" class="titulo_8b" Font-Bold="true" ForeColor="#042743" ></asp:Label> 
                <br>
                <asp:Label ID="Label76" runat="server" Text="¡Aquí tienes todas las herramientas necesarias para tu negocio!" class="texto_3b" 
                ForeColor="#929397" ></asp:Label> 
                </td>
                </tr>
                </table>
                <br>
                </td>
                </tr>
            </table>



		<div class="showcase-slider ancho_slide" style=""  >
			<div id="MS59d154dcb57d8" class="ms-skin-black-2 " >

				 				 
			<div class="ms-slide" >
			<div class="ms-thumb" >
            <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" >
            <tr>
            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink31" NavigateUrl="~/Share_Zarpe.aspx#videos"  runat="server" > 
            <asp:Image ID="Image21" runat="server" ImageUrl="~/Styles/images/zarpe_menu_1.png" class="ancho_imagen2" />
            <asp:Label ID="Label46" runat="server" Text="COMPARTIR<br>VIDEOS"  CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink> 
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top" style="margin-right:-10px; display: block;">
            <asp:HyperLink ID="HyperLink32" NavigateUrl="~/Share_Zarpe.aspx#productos" runat="server">
            <asp:Image ID="Image22" runat="server" ImageUrl="~/Styles/images/zarpe_menu_2.png" class="ancho_imagen2" /> 
            <asp:Label ID="Label47" runat="server" Text="COMPARTIR<br>PRODUCTOS"  CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink33" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
            <asp:Image ID="Image23" runat="server" ImageUrl="~/Styles/images/zarpe_menu_3.png" class="ancho_imagen2" /> 
            <asp:Label ID="Label49" runat="server" Text="COMPARTIR<br>SÚPER ALIMENTOS" style="width:92px;display:block;line-height: 14px!important;" 
            CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink54" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
            <asp:Image ID="Image36" runat="server" ImageUrl="~/Styles/images/zarpe_menu_4.png" class="ancho_imagen2" /> 
            <asp:Label ID="Label77" runat="server" Text="COMPARTIR<br>EVENTOS"  CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink55" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
            <asp:Image ID="Image38" runat="server" ImageUrl="~/Styles/images/zarpe_menu_5.png" class="ancho_imagen2" /> 
            <asp:Label ID="Label78" runat="server" Text="ACTIVA<br>TU NEGOCIO"  style="width:80px;display:block;line-height: 14px!important;"
            CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>


            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink34" NavigateUrl="~/Share_Zarpe.aspx#herramientas" runat="server">
            <asp:Image ID="Image24" runat="server" ImageUrl="~/Styles/images/zarpe_menu_6.png" class="ancho_imagen2" /> 
            <asp:Label ID="Label51" runat="server" Text="DESCARGAR<br>CONTENIDO"  CssClass="texto_menu" Font-Bold="true"></asp:Label><br><br>
            </asp:HyperLink>
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink35" NavigateUrl="~/Share_Zarpe.aspx#blog" runat="server">
            <asp:Image ID="Image25" runat="server" ImageUrl="~/Styles/images/zarpe_menu_7.png" class="ancho_imagen2" />
            <asp:Label ID="Label52" runat="server" Text="COMPARTIR<br>BLOG"  CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>

            <td class="ancho_imagen" ></td>

            <td align="center" valign="top">
            <asp:HyperLink ID="HyperLink36" NavigateUrl="~/Share_Zarpe.aspx#prospectos" runat="server">
            <asp:Image ID="Image26" runat="server" ImageUrl="~/Styles/images/zarpe_menu_8.png" class="ancho_imagen2" />
            <asp:Label ID="Label53" runat="server" Text="CONTROL DE<br>PROSPECTOS"  CssClass="texto_menu" Font-Bold="true"></asp:Label>
            </asp:HyperLink>
            </td>

            </tr>
            </table> 	                 
            </div>
			</div>
					
        
			<%--<div class="ms-slide" >
            <div class="ms-thumb" >
            <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" >
            <tr>
            <td class="ancho_imagen" ></td>
            </tr>
            </table> 

			</div>
			</div>--%>


			</div>		 
		</div>
    </td>
    </tr>
</table>    
		
		<script>
		    (window.MSReady = window.MSReady || []).push(function ($) {

		        "use strict";
		        var masterslider_57d8 = new MasterSlider();
		        // slider controls
		        masterslider_57d8.control('arrows', { autohide: true, overVideo: true });
		        masterslider_57d8.control('bullets', { autohide: true, overVideo: true, dir: 'h', align: 'bottom', space: 5, margin: 10 });
		        masterslider_57d8.control('thumblist', { autohide: false, overVideo: true, dir: 'h', speed: 17, inset: false, arrows: false, hover: false, customClass: '', align: 'bottom', type: 'thumbs', margin: 5, width: 100, height: 100, space: 5, fillMode: 'fill' });
		        masterslider_57d8.control('scrollbar', { autohide: false, overVideo: true, dir: 'h', inset: true, align: 'top', color: '#3D3D3D', margin: 10, width: 4 });
		        masterslider_57d8.control('slideinfo', { autohide: false, overVideo: true, dir: 'v', align: 'right', inset: false, margin: 20, size: 300 });
		        // slider setup
		        masterslider_57d8.setup("MS59d154dcb57d8", {
		            width: 499,
		            height: 539,
		            minHeight: 0,
		            space: 0,
		            start: 1,
		            grabCursor: true,
		            swipe: true,
		            mouse: true,
		            keyboard: false,
		            layout: "boxed",
		            wheel: false,
		            autoplay: false,
		            instantStartLayers: false,
		            mobileBGVideo: false,
		            loop: false,
		            shuffle: false,
		            preload: 0,
		            heightLimit: true,
		            autoHeight: false,
		            smoothHeight: true,
		            endPause: false,
		            overPause: true,
		            fillMode: "fill",
		            centerControls: true,
		            startOnAppear: false,
		            layersMode: "center",
		            autofillTarget: "",
		            hideLayers: false,
		            fullscreenMargin: 0,
		            speed: 20,
		            dir: "h",
		            parallaxMode: 'swipe',
		            view: "basic"
		        });

		        window.masterslider_instances = window.masterslider_instances || [];
		        window.masterslider_instances.push(masterslider_57d8);
		    });
		</script>

<script type="text/javascript" src='<%= System.Configuration.ConfigurationManager.AppSettings["WebPagePath"]%>/Styles/dist/slide/masterslider.min.js<%= System.Configuration.ConfigurationManager.AppSettings["WebVersion"] %>'></script>






<%--<div class="css-slider-wrapper ver_en_movil"></div>--%>
    



    


    <!-- Menu PC / Share --> 
    <table id="menuShare_PC" runat="server" width="100%" border="0" align="center" cellpadding="0" cellspacing="0" class="zarpe_pc"
    style=" background:#e6e7e9; height:120px; margin-bottom:20px; " >
    <tr>
    <td align="center">

    <!-- Bienvenido / Share --> 
    <table width="100%" border="0" align="center" cellpadding="0" cellspacing="0" style=" background:#ffffff!important; ">
        <tr>
        <td>

        <table width="85%" border="0" align="center" cellpadding="0" cellspacing="0" >
        <tr>
        <td align="right">
        <asp:Label ID="Label81" runat="server" Text="Bienvenido (a)" class="titulo_8b" ForeColor="#042743" ></asp:Label>
        <asp:Label ID="lbFirstName" runat="server" Text="Nombre" class="titulo_8b" Font-Bold="true" ForeColor="#042743" ></asp:Label> 
        <br>
        <asp:Label ID="Label73" runat="server" Text="¡Aquí tienes todas las herramientas necesarias para tu negocio!" class="texto_3b" 
        ForeColor="#929397" ></asp:Label> 
        </td>
        </tr>
        </table>
        <br><br>
        </td>
        </tr>
    </table>



        <table width="98%" border="0" align="center" cellpadding="0" cellspacing="0" style="max-width:1100px">
        <tr>
        <td align="center"> 
        <asp:HyperLink ID="HyperLink11" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#videos" runat="server">
        <asp:Image ID="Image10" runat="server" ImageUrl="~/Styles/images/zarpe_menu_1.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label66" runat="server" Text="COMPARTIR VIDEOS"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink12" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#productos" runat="server">
        <asp:Image ID="Image11" runat="server" ImageUrl="~/Styles/images/zarpe_menu_2.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label15" runat="server" Text="COMPARTIR PRODUCTOS"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink13" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
        <asp:Image ID="Image12" runat="server" ImageUrl="~/Styles/images/zarpe_menu_3.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label17" runat="server" Text="COMPARTIR<br>SÚPER ALIMENTOS"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink56" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
        <asp:Image ID="Image39" runat="server" ImageUrl="~/Styles/images/zarpe_menu_4.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label89" runat="server" Text="COMPARTIR EVENTOS"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink57" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#superalimentos" runat="server">
        <asp:Image ID="Image40" runat="server" ImageUrl="~/Styles/images/zarpe_menu_5.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label90" runat="server" Text="ACTIVA<br>TU NEGOCIO"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink14" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#herramientas" runat="server">
        <asp:Image ID="Image13" runat="server" ImageUrl="~/Styles/images/zarpe_menu_6.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label19" runat="server" Text="DESCARGAR CONTENIDO"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink15" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#blog" runat="server">
        <asp:Image ID="Image14" runat="server" ImageUrl="~/Styles/images/zarpe_menu_7.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label20" runat="server" Text="COMPARTIR<br>BLOG"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        <asp:HyperLink ID="HyperLink16" class="menu_padding" NavigateUrl="~/Share_Zarpe.aspx#prospectos" runat="server">
        <asp:Image ID="Image15" runat="server" ImageUrl="~/Styles/images/zarpe_menu_8.png" style="width:100%; max-width:60px;" /><br> 
        <asp:Label ID="Label27" runat="server" Text="CONTROL DE PROSPECTOS"  CssClass="texto_20" ForeColor="#728191" Font-Bold="true"></asp:Label>
        </asp:HyperLink> 

        </td>
        </tr>
        </table>
    </td>
    </tr>
    </table>






<header id="headInShare" runat="server" style=" display:none;"></header>





</ContentTemplate>
</asp:UpdatePanel>


<asp:ContentPlaceHolder ID="MainContent" runat="server">
</asp:ContentPlaceHolder>

</div>

<table align="center" border="0" cellspacing="0" cellpadding="0" style="width:100%;background:#ffffff; max-width:2000px; display:none;" >
        <tr>
        <td align="center">

<table align="center" border="0" cellspacing="0" cellpadding="0" style="width:100%; max-width:2000px; " >
        <tr>
        <td align="center">
        <asp:HyperLink ID="HyperLink8"  NavigateUrl="~/Opportunity_Zarpe.aspx" Target="_blank" runat="server">
        <asp:Image ID="Image4" runat="server" ImageUrl="~/Styles/images/zarpe_fondo29.jpg" CssClass="zarpe_pc" style="width:100%; max-width:2000px;"/> 
        <asp:Image ID="Image30" runat="server" ImageUrl="~/Styles/images/zarpe_fondo29b.jpg" CssClass="zarpe_movil" style="width:100%; max-width:2000px;"/> 
        </asp:HyperLink>
        </td>
        </tr>
</table>

        </td>
        </tr>
</table>


<!-- Banner 2 -->
<%--<div class="wrapper-home">

<asp:HyperLink ID="HyperLink7" NavigateUrl="~/Opportunity.aspx" runat="server">
<asp:Image ID="Image9" runat="server" ImageUrl="~/Styles/images/oportunidad_banner.jpg" CssClass="imagen-header no_ver_en_movil2"/>
<asp:Image ID="Image10" runat="server" ImageUrl="~/Styles/images/oportunidad_banner2.jpg" CssClass="imagen-header ver_en_movil"/>
</asp:HyperLink>

</div>--%>



<table align="center" border="0" cellspacing="0" cellpadding="0" style="width:100%; max-width:2000px;" >
<tr>
<td align="center">
<asp:HyperLink ID="HyperLink43" runat="server" NavigateUrl="https://hoy.zar.pe/aboutchris/" Target="_blank" >
<asp:Image ID="Image47" runat="server" ImageUrl="~/Styles/images/zarpe_fondo44.jpg" CssClass="imagen-header no_ver_en_movil2" />
<asp:Image ID="Image49" runat="server" ImageUrl="~/Styles/images/zarpe_fondo44_movil.jpg" CssClass="imagen-header ver_en_movil" />
</asp:HyperLink>


</td>
</tr>
</table>



<div class="banner_10" >
<table align="center" border="0" cellspacing="0" cellpadding="0" style="width:100%; max-width:2000px; height:200px;" >
        <tr>
        <td align="center"><br>


        <!-- Compartir -->
        <table width="90%" border="0" align="center" cellpadding="0" cellspacing="0" >
        <tr>
        <td align="left">

        <div class="ancho_footer1" >
                
                <asp:HyperLink ID="HyperLink38" runat="server" NavigateUrl="https://api.whatsapp.com/send?phone=51934732284&text=Hola!%20Quiero%20recibir%20más%20información%20" target="_blank" class="ver_en_movil2222">
                    <asp:Image ID="Image34" runat="server" ImageUrl="~/Styles/images/zarpe_whasap3.png" class="icono_social" />
                </asp:HyperLink>

                <asp:HyperLink ID="HyperLink50" runat="server" NavigateUrl="https://m.me/zarperu" target="_blank" class="ver_en_movil2222">
                    <asp:Image ID="Image35" runat="server" ImageUrl="~/Styles/images/zarpe_msn3.png" class="icono_social"/>
                </asp:HyperLink>

                <asp:HyperLink ID="footerHiperlink2" runat="server" NavigateUrl="https://www.facebook.com/zarpeconnosotros/" Target="_blank">
                    <asp:Image ID="Image1" runat="server" ImageUrl="~/Styles/images/zarpe_facebook.png" class="icono_social"></asp:Image>
                </asp:HyperLink>
                <asp:HyperLink ID="HyperLink17" runat="server" NavigateUrl="https://www.instagram.com/zar_pe/" Target="_blank">
                    <asp:Image ID="Image16" runat="server" ImageUrl="~/Styles/images/zarpe_instagram.png" class="icono_social"></asp:Image>
                </asp:HyperLink>
                <asp:HyperLink ID="HyperLink39" runat="server" NavigateUrl="https://www.youtube.com/channel/UCfNI9n5J0_xXJUJ4z2hAt_A" Target="_blank">
                    <asp:Image ID="Image31" runat="server" ImageUrl="~/Styles/images/zarpe_youtube.png" class="icono_social2"></asp:Image>
                </asp:HyperLink>
                <asp:Label ID="footerLabel2" runat="server" class="texto_3" Font-Bold="true" ForeColor="#1a5c8c" Text=" Síganos en nuestras redes"></asp:Label>
                <br>
        </div>

        <div class="ancho_footer2 no_ver_en_movil2" >
            <table width="100%" border="0" align="right" cellpadding="0" cellspacing="0" >
            <tr>
            <td align="right"><asp:Image ID="Image32" runat="server" ImageUrl="~/Styles/images/zarpe_mail.png" Width="30px"></asp:Image>
            </td>

            <td align="right" width="124px">
            <asp:Label ID="Label61" runat="server" class="texto_17" Font-Bold="true" ForeColor="#195b8d" Text="Contáctenos"></asp:Label><br>
            <asp:Label ID="Label62" runat="server" class="titulo_9" Font-Bold="true" ForeColor="#1b5b87" Text="info@zar.pe"></asp:Label>
            </td>
            </tr>
            </table>
        
        
        </div>



        </td>
        </tr>
        </table>



            <div class="footer-content__data txt-r" style=" display:none;">
                <span class="footer-content__data__title contact">
                    <asp:Label ID="lbReferenceMessageFooter" runat="server" Text="Usuario le ha referido a esta página"></asp:Label>
                </span>
                <br>
                <span class="footer-content__data__correo">
                     <asp:Label ID="lbReferenceEmailFooter" runat="server" Text="Usuario le ha referido a esta página"></asp:Label>
                </span>
            </div>


        <!-- Menu pie de pagina -->
        <div class="" style="text-align:center;">
            <div class="ver_en_movil" >

                <asp:Label ID="Label57" runat="server" class="texto_17" Font-Bold="true" ForeColor="#195b8d" Text="Contáctenos"></asp:Label>
                <asp:Label ID="Label58" runat="server" class="titulo_9" Font-Bold="true" ForeColor="#1b5b87" Text="info@zar.pe"></asp:Label>

                <table width="70%" border="0" align="center" cellpadding="0" cellspacing="0" >
                <tr>
                <td align="center"><hr style="background:#85a7c0!important; width:100%; "></td>
                </tr>
                </table>
                
                <asp:HyperLink ID="HyperLink25" NavigateUrl="~/PrivacyPolicy.aspx" runat="server">
                    <asp:Label ID="Label40" runat="server" Text="Políticas de privacidad" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink26" NavigateUrl="~/TermsandConditions.aspx" runat="server">
                <asp:Label ID="Label41" runat="server" Text="Términos y condiciones" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink27" NavigateUrl="~/PolicyPersonalData.aspx" runat="server">
                <asp:Label ID="Label42" runat="server" Text="Políticas sobre el Uso de datos personales y derechos ARCO" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink28" NavigateUrl="~/DataProtection.aspx" runat="server">
                <asp:Label ID="Label43" runat="server" Text="Protección de Datos" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink29" NavigateUrl="~/Cookiepolicy.aspx" runat="server">
                <asp:Label ID="Label44" runat="server" Text="Uso de Cookies" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink30" NavigateUrl="~/LibrodeReclamaciones.aspx" runat="server">
                <asp:Label ID="Label45" runat="server" Text="Libro de reclamaciones" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                <br>
                <asp:HyperLink ID="HyperLink24" NavigateUrl="#" runat="server">
                            <asp:Label ID="Label39" runat="server" Text="BLOG" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>
                
                <br>
                <asp:HyperLink ID="HyperLink52" NavigateUrl="~/ContactUs.aspx" runat="server">
                            <asp:Label ID="Label71" runat="server" Text="Contacto" ForeColor="#165c8d" class="texto_4" Font-Bold="true"></asp:Label>
                </asp:HyperLink>


                <table width="70%" border="0" align="center" cellpadding="0" cellspacing="0" >         
                <tr>
                <td align="center"><hr style="background:#85a7c0!important; width:100%; "></td>
                </tr>
                </table>

            </div>

            <div class=" footer-content__data--join ocultar_en_movil" style="color:#165c8d; ">
            <br><br>    
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterPrivacyPolicy" NavigateUrl="~/PrivacyPolicy.aspx" runat="server">
                    <asp:Label ID="lbFooterPrivacyPolicy" runat="server" Text="Politicas de privacidad" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterTermsandConditions" NavigateUrl="~/TermsandConditions.aspx" runat="server">
                    <asp:Label ID="lbFooterTermsandConditions" runat="server" Text="Términos y condiciones" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="footerHiperlink6" NavigateUrl="~/PolicyPersonalData.aspx" runat="server">
                    <asp:Label ID="Label38" runat="server" Text="Políticas sobre el Uso de datos personales y derechos ARCO" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterDataProtection" NavigateUrl="~/DataProtection.aspx" runat="server">
                    <asp:Label ID="lbFooterDataProtection" runat="server" Text="Protección de Datos" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterCookiepolicy" NavigateUrl="~/Cookiepolicy.aspx" runat="server">
                    <asp:Label ID="lbFooterCookiepolicy" runat="server" Text="Uso de Cookies" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterLibrodeReclamaciones" NavigateUrl="~/LibrodeReclamaciones.aspx" runat="server">
                    <asp:Label ID="lbFooterLibrodeReclamaciones" runat="server" Text="Libro de reclamaciones" Font-Bold="true" ForeColor="#165c8d" Font-Size="12px"></asp:Label>
                    </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="lnkFooterBlog" NavigateUrl="#" runat="server">
                            <asp:Label ID="lbFooterBlog" runat="server" Text="BLOG" ForeColor="#185c8d" Font-Bold="true" Font-Size="12px"></asp:Label>
                     </asp:HyperLink>
                </span>|
                <span class="texto_7">
                    <asp:HyperLink ID="HyperLink53" NavigateUrl="~/ContactUs.aspx" runat="server">
                            <asp:Label ID="Label72" runat="server" Text="Contacto" ForeColor="#185c8d" Font-Bold="true" Font-Size="12px"></asp:Label>
                     </asp:HyperLink>
                </span>
                <br>
                <%--<span id="siteseal"><script async type="text/javascript" 
                src="https://seal.godaddy.com/getSeal?sealID=BrHxd1TkJRUoyan5LaQK11yuXTucjcSfclHum2BoOInDzsi5afbqLVbTXdfm"></script></span>
                <script type="text/javascript" src="https://cdn.ywxi.net/js/1.js" async></script>--%>


                
            </div>
            
            <br>
            <asp:Label class="texto_4" ID="footerLabel4" runat="server" Text="Todos los derechos reservados" Font-Bold="true" ForeColor="#165c8d"></asp:Label>
            <br>
            <asp:Label class="texto_4" ID="Label29" runat="server" Text="Zarpe" Font-Bold="true" ForeColor="#165c8d"></asp:Label>
            <asp:Image ID="Image33" runat="server" ImageUrl="~/Styles/images/zarpe_r.png" Width="8px" style="margin-top:2px; margin-left:-4px"></asp:Image>
            <asp:Label class="texto_4" ID="Label59" runat="server" Text=" 2018" Font-Bold="true" ForeColor="#165c8d"></asp:Label>
            <br><br>
        </div>



        </td>
        </tr>
</table>
</div>


<footer class="footer-container" >

</footer>



<asp:Panel ID="popupCountries" runat="server" ClientIDMode="Static" class="modal fade in modal--home" tabindex="-1" 
role="dialog" aria-labelledby="myModalLabel" >

<%--    <div class="modal fade in modal--home" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel">--%>
      <div class="modal-dialog" >
        <div class="modal-content">
          <div class="wrapper" >
            <div class="modal-header">
              <button class="close" type="button" data-dismiss="modal" aria-label="Close" onclick=" $('#popupCountries').bPopup().close(); ">
                <div class="span" aria-hidden="true">x</div>
              </button>
            </div>
            <div class="modal-body">
              <div class="col-md-5">
                      <br>
                      <asp:Label ID="Label3" runat="server" Text="Usuarios Registrados" Font-Bold="True" class="texto_7"></asp:Label><br> 
                      <asp:Label ID="Label13" runat="server" Text="Selecciona el país donde te encuentras" Cssclass="no_ver_en_movil2 texto_7" ></asp:Label>
                

                <div class="select__countries">
                  <ul>

                        <asp:DataList ID="dtlCountriesPopup" runat="server" ClientIDMode="Static" RepeatDirection="Horizontal" RepeatLayout="Flow">
                        <ItemTemplate>

                        <asp:HiddenField ID="hdCountryID" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryID") %>' Visible="false" />
                        <asp:HiddenField ID="hdCountryName" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' Visible="false" />

                        <li class="margen_banderas" >
                            <asp:LinkButton ID="lnkCountry" runat="server" OnClick="lnkCountry_Click">
                            <asp:Image ID="imgItemCountry" runat="server" Width="28px" 
                            ImageUrl='<%# "~/Styles/images/Country/"+DataBinder.Eval(Container.DataItem, "CountryID")+".png" %>' />
                            &nbsp;
                            <asp:Label ID="lbItemCountry" runat="server" Text='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' class="texto_7"></asp:Label>
                            </asp:LinkButton>
                        </li>

                        </ItemTemplate>
                        </asp:DataList>

                  </ul>

                </div>
                <br />
                 <span>
                      <asp:Label ID="Label22" runat="server" CssClass="no_ver_en_movil2 texto_7" Text="Bienvenidos a ZARPE"  
                      Font-Bold="True" ForeColor="#666666"></asp:Label>
                 </span>
              </div>
              <div class="col-md-7 ">
                    <br>
                    <asp:Label ID="Label24" runat="server" Text="Usuarios Nuevos <br />" Font-Bold="True"  class="texto_7"></asp:Label>
                    <asp:Label ID="Label8" runat="server" Text="Si aún no estamos en tu país" Cssclass="no_ver_en_movil2 texto_7"></asp:Label>
                          <%--<asp:HyperLink ID="HyperLink33" runat="server"></asp:HyperLink>--%>
                    <asp:Label ID="Label25" runat="server" Text="Regístrate" Cssclass="no_ver_en_movil2 texto_7" Font-Bold="True"></asp:Label>
                <div class="no_ver_en_movil2">
                    <asp:Label ID="Label7" runat="server" Text="Y conoceras primero las noticias de Zarpe en tu país." class="texto_7"></asp:Label>
                </div>
                
                 <div id="Div2" runat="server">
                 
                       <div class="ancho_zarpe30">
                       <asp:TextBox ID="txtEmailRegisterPopup" runat="server" ClientIDMode="Static" 
                       class="campo_texto_zarpe_2  texto_7" 
                       data-msg-required="Please enter your email address." placeholder="Correo electrónico" ></asp:TextBox>
                       </div>

                       <div class="ancho_zarpe30" style="margin-top: 8px;">
                       <a class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false" 
                       runat="server" visible ="false">
                        <span>
                            <asp:TextBox ID="hdCountryIDPopup" runat="server" ClientIDMode="Static" style="display:none;"   />
                            <asp:Label ID="lblCurrentCountryPopup" runat="server" ClientIDMode="Static" Text="Selecciona tu país" ></asp:Label>
                            <asp:Image ID="imgCurrentCountryPopup" runat="server" ClientIDMode="Static" Width="22px" style=" margin-left:5px;" />
                            <span class="caret"></span>
                        </span>
<%--                        <span class="hide">
                            <asp:Label ID="Label8" runat="server" Text="El Salvador "></asp:Label>
                            <span class="flag-icon flag-icon-sv flag-icon--caret"></span>
                            <span class="caret"></span>
                        </span>--%>
                        <ul class="dropdown-menu dropdown-menu--black ">
                        <asp:DataList ID="dtlCountriesAllPopup" runat="server" ClientIDMode="Static" RepeatLayout="Flow" RepeatDirection="Horizontal">
                        <ItemTemplate>

                        <asp:HiddenField ID="hdCountryID" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryID") %>' Visible="false" />
                        <asp:HiddenField ID="hdCountryName" runat="server" Value='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' Visible="false" />

                        <li>
                            <a onclick='<%# "AssignedCountryPopup("+ DataBinder.Eval(Container.DataItem, "CountryID") +",\""+ DataBinder.Eval(Container.DataItem, "CountryName") + "\",\"" + System.Configuration.ConfigurationManager.AppSettings["WebPagePath"] + "/Styles/images/Country/Flags/"+DataBinder.Eval(Container.DataItem, "CountryISOLetter")+".png" + "\");" %>' >
                            <span class="flag-icon">
                            <asp:Image ID="imgItemCountry" runat="server" ImageUrl='<%# "~/Styles/images/Country/Flags/"+DataBinder.Eval(Container.DataItem, "CountryISOLetter")+".png" %>' />
                            </span>
                             &nbsp; &nbsp;
                            <asp:Label ID="lbItemCountry" runat="server" Text='<%# DataBinder.Eval(Container.DataItem, "CountryName") %>' ></asp:Label>
                            </a>
                        </li>

                        </ItemTemplate>
                        </asp:DataList>
                        </ul>
                        </a>
                      
                        <asp:DropDownList ID="ddlCountriesAllPopup" runat="server" ClientIDMode="Static" class=" select_2">
                        </asp:DropDownList>               
                        </div>


                    <div class="ancho_zarpe30 bajar_movil">
                    <asp:LinkButton ID="lnkRegisterPopup" runat="server" ClientIDMode="Static" Text="Registrarme" 
                    style="background:#a4cde1;margin:5px;padding:9px;width:130px!important;border-radius:30px; padding-left:12px;padding-right:12px;" 
                    ValidationGroup="ValidateRegisterPopup" OnClick="lnkRegisterPopup_Click" class="texto_3" ForeColor="#052941">
                    </asp:LinkButton>
                    </div>


                    <table width="100%">
                    <tr>
                    <td class="alinear_en_movil">
                        <asp:RequiredFieldValidator ID="frvCountryIDPopup" runat="server" ControlToValidate="hdCountryIDPopup" ErrorMessage="Seleccione su País" Font-Bold="True" 
                        CssClass="mover_izq2" ForeColor="Red" SetFocusOnError="True" ValidationGroup="ValidateRegisterPopup" ></asp:RequiredFieldValidator>

                        <br />
                        <asp:RequiredFieldValidator ID="rfvEmailRegisterPopup" runat="server" ControlToValidate="txtEmailRegisterPopup" ErrorMessage="Ingrese Email" Font-Bold="True" 
                        CssClass="mover_izq2" ForeColor="Red" SetFocusOnError="True" ValidationGroup="ValidateRegisterPopup" ></asp:RequiredFieldValidator>
                        <br />
                        <asp:RegularExpressionValidator ID="revEmailRegisterPopup" runat="server" ControlToValidate="txtEmailRegisterPopup" ErrorMessage="Ingrese Email Valido" Font-Bold="True" 
                         ForeColor="Red" SetFocusOnError="True" ValidationGroup="ValidateRegisterPopup"
                        Display="Dynamic" ValidationExpression="\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*" ></asp:RegularExpressionValidator>
                    </td>
                    </tr>
                    </table>

                
                    <span>
                      <asp:Label ID="Label9" runat="server" CssClass="ver_en_movil " 
                      Text="Bienvenidos a ZARPE"  Font-Bold="True" ForeColor="#666666"></asp:Label>
                    </span>
                </div>


                <div class="col-md-6 col-md-offset-3"><br><div class="no_ver_en_movil2"> <br></div>
                <asp:Image ID="imgGanolifePopup"  runat="server" ImageUrl="~/Styles/images/zarpe_logo2.jpg" CssClass="no_ver_en_movil2" 
                style="margin-top:-30px" Width="160px" /><div class="no_ver_en_movil2"> <br><br></div>
                </div>
                <div class="form__selects" >
                  <div class="col-md-6 col-xs-6">
                     <a class="dropdown-toggle" data-toggle="dropdown" role="button" aria-haspopup="true" aria-expanded="false">
                     <span>
                     <asp:Label ID="Label30" runat="server" CssClass="no_ver_en_movil2" Text="Selecciona tu Idioma"></asp:Label> 
                     <asp:Label ID="Labe548" runat="server" CssClass="ver_en_movil" Text="Idioma"></asp:Label> 
                     <span class="caret subir_en_tablet4"></span></span>
                     <span class="hide">
                     <asp:Label ID="Label48" runat="server" Text="Español"></asp:Label> 
                     <span class="caret"></span></span>
                     <ul class="dropdown-menu dropdown-menu--black mover_izq4">
                        
                        <li>
                            <asp:HyperLink ID="HyperLink210" runat="server" NavigateUrl="#">
                                <asp:Label ID="Label34" runat="server" Text="Ingles" class="texto_7"></asp:Label>
                            </asp:HyperLink>
                        </li>
                        <li>
                            <asp:HyperLink ID="HyperLink211" runat="server" NavigateUrl="#">
                                <asp:Label ID="Label482" runat="server" Text="Español" class="texto_7"></asp:Label>
                            </asp:HyperLink>
                        </li>
                       <%--   <li>
                            <asp:HyperLink ID="HyperLink220" runat="server" NavigateUrl="#">
                                <asp:Label ID="Label49" runat="server" Text="Francés"></asp:Label>
                            </asp:HyperLink>
                        </li>
                           <li>
                            <asp:HyperLink ID="HyperLink221" runat="server" NavigateUrl="#">
                                <asp:Label ID="Label59" runat="server" Text="Portugués"></asp:Label>
                            </asp:HyperLink>
                        </li>--%>
                        
                     </ul>
                     </a>
                  </div>
                  <div class="col-md-6 col-xs-6">
                      <asp:HyperLink ID="lnkPopupCountriesHomeZarpe" runat="server" class="link-ganolife" NavigateUrl="~/Home_Zarpe.aspx">
                          <asp:Label ID="Label50" runat="server" Text="Ir a ZARPE" class="texto_7"></asp:Label>
                      </asp:HyperLink>
                  </div>
                </div>
                <br><br>
              </div><br class="clear"><br>
            </div>
          </div>
        </div>
      </div>
<%--    </div>--%>

</asp:Panel>


	 <%-- Gracias por registrarte --%>
    <asp:Panel ID="popupThankYou" runat="server" BackColor="#f7f7f7" Height="280px" CssClass="PopupStyle ancho_popup" 
    style="background:#ffffff; box-shadow: 5px 5px 20px 3px rgba(0,0,0,0.2); padding:14px; " ClientIDMode="Static">
        <div style="padding:6px; float:right">
            <asp:HyperLink ID="HyperLink2" runat="server" onclick=" $('#popupThankYou').bPopup().close(); ">
            <asp:Image ID="Image5" runat="server" ImageUrl="~/Styles/images/zarpe_x.jpg" />
            </asp:HyperLink>
        </div>
        
         
        <div style="width:100%; padding:20px; border:1px solid #8193a1; text-align:center ">

        <asp:Image ID="Image6" runat="server" ImageUrl="~/Styles/images/zarpe_logo2.jpg" Width="170px"/>
        <br>
        <asp:Label ID="lbMessageRegisterOK" runat="server" Text="Gracias por registrarte"  class="titulo_7" ></asp:Label><br>
        <asp:Label ID="lbMessageRegisterSendMail" runat="server" class="texto_16" 
        Text="En breve recibirás un correo de confirmación en la bandeja de tu correo electrónico" ></asp:Label>
        <br><br>

        <asp:HyperLink ID="lnkPopupRegister" runat="server" NavigateUrl="~/Home_Zarpe.aspx" class="boton_celeste" >
        <asp:Label ID="Label63" runat="server" ForeColor="#001e3a" CssClass="texto_3" Text="Continuar" ></asp:Label>
        </asp:HyperLink>

        <br>
        </div>
        <br>
</asp:Panel>




<div id="fb-root"></div>

<script>
(function (d, s, id) {
        var js, fjs = d.getElementsByTagName(s)[0];
        if (d.getElementById(id)) return;
        js = d.createElement(s); js.id = id;
        js.src = "//connect.facebook.net/es_LA/sdk.js#xfbml=1&version=v2.7&appId=1593903597522194";
        fjs.parentNode.insertBefore(js, fjs);
} (document, 'script', 'facebook-jssdk'));</script>


<script type="text/javascript">
    $(document).ready(function () {

        $('span > li').unwrap();

    });
</script>








</form>
</body>
      
</html>

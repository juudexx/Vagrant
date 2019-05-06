---


---

<p>OBJECTIU: FER SERVIR SCRIPT BASH PER APROVISIONAR UNA VM INSTANCIADA AMB VAGRANT.</p>
<p>En aquesta pràctica faràs servir Vagrant per automatitzar la creació d’una màquina virtual en VirtualBox amb la darrera versió d’Ubuntu Server, amb 2GB de memòria. L’hauràs de provisionar amb un script per tal que aquesta MV contingui una pila LAMP. Per controlar la base de dades també es demana que quedi instal·lada l’aplicació adminer  <a href="https://github.com/vrana/adminer">https://github.com/vrana/adminer</a></p>
<p>HAURÀS DE LLIURAR:</p>
<ul>
<li>
<p>Document tècnic amb la descripció dels passos que has dut a terme per a la implementació de la VM i l’aprovisionament. Especialment cada comanda Vagrant que s’ha fet servir i per què.</p>
</li>
<li>
<p>L’adreça del repositori GitHub on puges el Vagrantfile i on ha de constar el document tècnic en format Markdown. Pots fer servir un editor online.</p>
</li>
<li>
<p>L’aprovisionament es fa mitjançant un script de bash i s’ha d’indicar amb comentaris què es fa en cada comanda.</p>
</li>
<li>
<p>Check un cop s’ha fet la tramesa en què es</p>
</li>
<li>
<p>mostra el repositori</p>
</li>
<li>
<p>generació de les VM mitjançant Vagrantfile.</p>
</li>
<li>
<p>Connexió a la applicació adminer i gestió d’una BBDD</p>
</li>
</ul>
<p>Lo primero que hay que hacer es crear una carpeta donde queramos crear la MV.</p>
<p>Por ejemplo, en nuestro caso la hemos creado en el Escriptori:</p>
<p>mkdir vagrant</p>
<p><img src="https://lh3.googleusercontent.com/CeUiiKuDb5_fsNC2qiCSKnQqArHoSVy_3yiVwB4je4qAgcS6c83cJK8GKKYqRuzddLSOlrWH9xPM3x4i5ScSzjAoW01KZINxqxlKNnis5jq56pfqe9QQhCF_qfc0_LG6362TfPNY" alt=""></p>
<p>A continuación entramos en la carpeta creada y ejecutamos:</p>
<p><img src="https://lh4.googleusercontent.com/ydDFEfNBoEB86K3n1EKR_WItWqzWTx1DAvTi9mO3ZhroYCLpD0ab1VQ-ticwv-PAziy0z1vMpPchsilL9_17YM4OUYFFVRGezT_V38ymZlZqqwWAH0N_nqMt5E7gbuC3okntb--I" alt=""></p>
<p>Añadimos la última versión de ubuntu server:</p>
<p><img src="https://lh4.googleusercontent.com/FAuV7I_MPDPJKK1t5OwC9tq1lPF0uFIB0w-tSlPKxwkNKn9X2KtYFtN8tcV9OCeIEpRPDhJ0EyrPL6FWduvneT-iXWC1OQMZbz6tlrAmOAwUrgqA5sKcGaFOayM7Qb1q6xZF5WzE" alt=""></p>
<p>Para poder iniciar la mv debemos modificar el archivo Vagrantfile y cambiar base por:</p>
<p><img src="https://lh6.googleusercontent.com/b0MO4f5oSQ6ROhce_ZfFgpKx03o4skmE9101TCPPjmD4UAN1efZn72y21zCRcj_55WllXAjuWOLosHH4HvDZWkofewZH_n8p--m-Rg7x27Ye72vmb2IZWwx4HLWYBSl6ebh6Vqg5" alt=""></p>
<p>También para darle 2GB de memoria lo hacemos dentro de este fichero:</p>
<p><img src="https://lh4.googleusercontent.com/nSPz7poINtIxpYN8g7j5VBMugMKm9QJnjIIxILHlTppgoh1MPhq1MK7LvvSf82t_djztJ6vjueg0QC3Vfi5mOpB37NIlBi_g3TaAG_7GGMsy6-0BjrXvTy5avaVzkTBiklGduKUr" alt=""></p>
<p>Para poder instalar programas debemos descomentar esta linea y</p>
<p><img src="https://lh3.googleusercontent.com/NoIIl0XGseI65FXXloxVpKHAvRF-miXzflH5_NT2PuPDWCB2STU92F5QJ-usk6lP7otKJNsX07Nj_FwRAe-ZkwTYQabUTmlCQ8Kwyy810NYInDFPSXe7s48K54xmahcJ6OaR2stz" alt=""></p>
<p>Ejecutamos este comando para poder iniciar la mv:</p>
<p><img src="https://lh4.googleusercontent.com/Iy-x4rpS5KSVnLDxM-Qlll7y29Y4Yr4n-KGwhy7Wb3RXgb_EB36FLdETZ8o7qq_jMl_kvf0dGFbOeEILY42XlvQydRV7tr3LCvcMh7aIsbquFh1BrAwfikuvPPCBviFuq7HGQVUW" alt=""></p>
<p>Comprobamos que funciona el ssh con la mv:</p>
<p><img src="https://lh4.googleusercontent.com/9ynfH5sMNRyPhEVLdNIPhp4BC8BcXpRfSwtbxTpZSv5vnMoGe4ozBfS-Fbc2D7Rs6jmH2g9Vp2pdg8-Ti76lVTzCo8qPFPax8vDGllUm6sCJ0BrcIMaQllVtTrcjLMYaXCsWKNfh" alt=""></p>
<p><img src="https://lh3.googleusercontent.com/X2LcqGeab3ZN8c7nCWlqu1e6ORORk-w4U4REVpTuJuadhqrEnBaSUa2A0yRT664Ob2Oqqs5ITuuzQFWLe9snFGxlHL1gBhJD2K-TF_ydQ5H7Je3MP41IWzEHNgGzZdzbosWzA_Zz" alt=""></p>


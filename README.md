<h1>Implementando fortigate com funcionalidade de SD-WAN</h1>

<h2>Descrição</h2>
O projeto consiste em criar um firewall FortiGate do zero, configurar as interfaces, adicioná-las a uma SD-WAN e criar um load balancer para garantir alta disponibilidade na internet.
<br />


<h2>Ferramentas utilizadas</h2>

- <b>EVE-NG</b> 
- <b>FORTIGATE</b>
- <b>Forti OS</b>

<h2>Ambientes usados</h2>

- <b>FORTIGATE</b> (21H2)

<h2>Como foi feito:</h2>

<p align="center">
Topologia base: <br/>
  <br>
<img src="https://i.imgur.com/RVqWBXS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
 <br>
 Configurando portas do firewall para acesso de administradores: <br/>
  <br>
<img src="https://i.imgur.com/k9TsLAh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <img src="https://i.imgur.com/J34oWiL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Configurando uma rede LAN dentro do Fortigate: <br/>
  <br>
 <img src="https://i.imgur.com/p9XSiCv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Configurando interface WAN para simular um link de internet: <br/>
  <br>
 <img src="https://i.imgur.com/UfeSms9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Configurando segunda interface WAN para simular outro link de internet: <br/>
  <br>
 <img src="https://i.imgur.com/16RSAg6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Criando SD-WAN e adicionando interfaces WAN para realizar o load balancer: <br/>
  <br>
 <img src="https://i.imgur.com/VC6V2x3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
  SD-WAN criado: <br/>
   <br>
 <img src="https://i.imgur.com/kQRCXpM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Criando rota estática e adicionado o SD-WAN:  <br/>
  <br>
 <img src="https://i.imgur.com/mWmZCKn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Criando regra no Firewall para permitir a saída da internet: <br/>
  <br>
 <img src="https://i.imgur.com/RsbmiHx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
 Adicionando serviços de segurança na regra do firewall: <br/>
 <img src="https://i.imgur.com/9bW1fmJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

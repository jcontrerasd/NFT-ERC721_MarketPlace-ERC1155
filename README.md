# NFT-ERC721_MarketPlace-ERC1155

# Creación de NFT ERC-721 y Smart Contract ERC1155 Market Place para venta y comprar ese NFT ERC721


**Nombre del Contrato MemoriaUrbanToken (MUT).**
Significado: Memorias Urbanas Token (MUT) es una colección de NFTs que retrata la historia de ciudades a lo largo del tiempo. Estos NFTs son creaciones únicas que representan momentos específicos de la evolución urbana. Creados por artistas, los MUT fusionan arte y patrimonio cultural. Son miradas al pasado que muestran cómo las ciudades han cambiado y celebran su diversidad. 
Los MUT son  más que  tokens digitales; son **obras de arte históricamente valiosas que permiten a los coleccionistas explorar y apreciar la historia urbana**.

### Casos de Uso ###

* **Colección de Arte Urbano:** Un coleccionista apasionado por la historia de las ciudades adquiere varios Memorias Urbanas Tokens (MUT) que representan momentos icónicos de diferentes urbes a lo largo del tiempo. Estos NFTs incluyen imágenes de antiguos edificios, calles, y cambios arquitectónicos a lo largo de los años. A medida que expande su colección, el coleccionista se sumerge en la narrativa visual de la evolución urbana, apreciando la fusión de arte y **patrimonio cultural**.

* **Exposición Digital**: Un museo de arte urbano organiza una exposición digital titulada "Memorias Urbanas: Ciudades en Transformación". Utilizan MUT para mostrar cómo las ciudades han cambiado con el tiempo a través de obras de artistas locales e internacionales. Los visitantes pueden explorar estas representaciones visuales de la historia urbana a través de NFTs en una plataforma en línea. La exposición ofrece una experiencia inmersiva que resalta la importancia de preservar y apreciar el patrimonio urbano. Los MUT se convierten en una forma única de conectar a las personas con el pasado de las ciudades y su diversidad artística.


# Se crean dos contratos
### 1.- MemoriaUrbanToken (Address [0x69e9A8db9dE48A77E404E045f06a4D224875376e](https://goerli.etherscan.io/address/0x69e9a8db9de48a77e404e045f06a4d224875376e#code)) ###

El contrato crea un token ERC721 llamado MemT (MUT). El contrato puede ser utilizado para crear nuevos tokens, aprobar la custodia del NFT a un contrato que permita custodiar el NFT y comercializarlo.

 <img width="1381" alt="image" src="https://github.com/jcontrerasd/NFT-ERC721_MarketPlace-ERC1155/assets/27821228/39b4acec-1617-4a1f-8a4c-109e42c275ba">



### Read Contract ###

    **1. balanceOf :** Devuelve la cantidad de un token que posee una dirección.

    **2. getApproved :** Devuelve la dirección que está autorizada para transferir un token en nombre de otra dirección.

    **3. isApprovedForAll :** Devuelve si una dirección está autorizada para transferir todos los tokens en nombre de otra dirección.

    **4. name :** Devuelve el nombre del token.

    **5. ownerOf :** Devuelve la dirección del propietario de un token.

    **6. supportsInterface :** Devuelve si un contrato implementa una interfaz.

    **7. symbol :** Devuelve el símbolo del token.

    **8. tokenURI :** Devuelve la URI del token.


### Write Contract ###

    **1. approve :** Establece una cantidad de valor de tokens como la asignación del gastador sobre los tokens de la persona que llama. 


### 2.- MarketplaceContract (Address [0x236648B702329C27Ab8f879C7477999290C893A6](https://goerli.etherscan.io/address/0x236648b702329c27ab8f879c7477999290c893a6#code)) ###
Corresponde a un MarketPlace que permite a los usuarios comprar y vender tokens ERC721. En resumen permite comprar y vender tokens ERC721.


<img width="1387" alt="image" src="https://github.com/jcontrerasd/NFT-ERC721_MarketPlace-ERC1155/assets/27821228/490c7815-a768-4f13-bf26-89c2c48f4a0b">

### Read Contract ###

    **1._itemsForSale :** Variable de estado que cuenta el número de NFTs en venta.
    
    **2.balanceOf : ** Devuelve la cantidad de un token que posee una dirección.
    
    **3.balanceOfBatch :**Devuelve la cantidad de un token que poseen varias direcciones.
    
    **4.getPrice :** Devuelve el precio de un NFT en wei.
    
    **5.isApprovedForAll :** Devuelve si una dirección está aprobada para transferir tokens en nombre de otra dirección.
    
    **6.supportInterface :** Devuelve si un contrato implementa una interfaz ERC721.
    
    **7.uri :** Devuelve la URI de un NFT.

### Write Contract ###

    **1.buyToken :** Compra un NFT ERC721 del mercado, pagando el precio especificado por el vendedor.
    
    **2.onERC721Received :** Recibe un NFT ERC721 en el contrato, verificando que el remitente está autorizado para transferirlo.
    
    **3.safeBatchTransferFrom :** Transfiere un lote de tokens ERC1155 de una dirección a otra de forma segura, verificando que la transferencia es válida y que el receptor tiene suficiente saldo.
    
    **4.safeTransferFrom :** Transfiere un token ERC721 de una dirección a otra de forma segura, verificando que la transferencia es válida y que el receptor tiene suficiente saldo.
    
    **5.setApprovalForAll :** Aprueba a una dirección para transferir todos los tokens ERC721 en nombre de otra dirección, otorgando permiso a un mercado para vender los tokens ERC721 de un usuario.
    
    **6.setSale :** Pone un NFT ERC721 a la venta en el mercado, especificando el precio al que se quiere vender.
    
    **7.unsetSale :** Elimina un NFT ERC721 de la venta en el mercado, permitiendo al propietario eliminarlo en cualquier momento.



### TRANSFERENCIA DE TOKEN : 
Se envió Tokens a la Addres 0xdE7F9087CfD6B3239E0F5c598847c2009c8FeF33 ([Hash Transacción](https://goerli.etherscan.io/tx/0x594669754b116c46187d4912ff3064d066fb481f6666804edd9b08a56ea7a8a1)) ###

![image](https://github.com/jcontrerasd/NewTokenSTT/assets/27821228/9fd21410-1ba8-428a-9f7b-ba2aac71680d)

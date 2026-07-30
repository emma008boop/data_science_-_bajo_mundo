Para entender como funciona un crypto banco, primero debemos entender [[Como funciona un Banco?]] para entender el negocio e identificar algunos huecos que pueden pasar cuando no tenermos un esquema bien estructurado.

## Como cambia un crypto banco el esquema de un banco tradicional?

Un criptobanco reemplaza al intermediario que en ese modelo es un banco; por un Smart Contract ejecutado en la blockchain.


![[Pasted image 20260725135943.png]]

Como vemos en la grafica, no hay una infraestructura fisica ni miles de empleados administrando creditos; el margen de intermediacion se reduce. Tambien vemos que hay una distribucion directa; si el prestatario paga un 8% de interes, casi la totalidad de ese 8% va directamente a los depositantes


# Las 3 columnas del Negocio 

## La captacion y los prestamos

**Colaterizacion (La garantia):** En el mundo real, si no pagas un credito, el banco te embarga la casa. En la blockchain no hay DNI ni cobradores. ¿Como se soluciona?; con #sobrecolaterizacion.

Ejemplo: Si quieres pedir un prestamo de 1000 USD en Stablecoins, el smart contract te exigira depositar como garantia el equivalente a 1,500 USD en Bitcoin o Ethereum. Si el valor de tu garantia cae demasiado por la volatidad del mercado, el contrato liquida automaticamente tu garantia para proteger el dinero de los depositantes

Ahora, por que alguien pediria un prestamo de 1000 USD cuando le pedimos 1500 de garantia?

Pongamoslo asi, imaginate comprar un 1 BTC a $30,000 como inversion a largo plazo. De repente necesitas $10,000 en efectivo para una emergencia o para pagar un gasto personal. Tienes dos opciones:
- Vender tu Bitcoin: Solucionas tu problema, pero pagas impuestos por la venta y pierdes la oportunidad de ganar dinero si bitcoin sube 100,000 en el futuro.
- Pedir un prestamo colaterizado: Entregas tu Bitcoin como garantia al Smart Contract, recibes los 10,000 en Stablecoins (USD), gastas ese dinero y, cuando devuelves los 10,000 (mas intereses), recuperas tu Bitcoin intacto. Si tu Bitcoin subio de precio en ese tiempo, la garantia sigue siendo tuya

# El ratio de colaterizacion

En el mundo tradicional, un banco revisa tu historial crediticio, tu nomina y tus ingresos antes de darte el dinero.

En la blockchain no hay historial crediticio ni identidades reales. El smart contract no sabe quien eres, solo ve una billetera digital. Como no te puede demandar ni embargar el sueldo si no pagas, exige #Sobrecolaterizacion (Dejar mas dinero del que pides).

![[Pasted image 20260725160626.png]]

### Que pasa si el mercado cae?

Por esto se pide mas de lo que prestas, ya que el Smart Contract debe de tomar un valor aproximado de cuanto puede llegar a caer la moneda teniendo un margen en el riesgo. En caso de que caiga a un porcentaje de Ratio 120% se activa la liquidacion y el Smart Contract vende automaticamente lo restante de ETH al mercado

![[Pasted image 20260725161159.png]]

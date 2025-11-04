# ENTREGA ÚNICA - Reto 01

> Exporta este archivo como **PDF único** con nombre:  
> `apellido1_apellido2_nombre_FHW01_Tarea`  *(sin ñ ni tildes)*

## Índice

- [Portada](#portada)
- [1. Introducción](#1-introduccion)
- [2. Conectores internos (energía)](#2-conectores-internos-energia)
- [3. Conectores de datos](#3-conectores-de-datos)
- [4. Slots de expansión](#4-slots-de-expansion)
- [5. Conectores externos](#5-conectores-externos)
- [6. Bibliografía](#6-bibliografia)

<a id="portada"></a>
## Portada
# Reto 1 — Investigación_Desarrollo_Conectores_Slots

**Módulo:** Fundamentos de Hardware (ASIR)  
**Alumno/a:** Abraham Aparicio Moreno 
**Curso:** 2025/26

![Portada](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/00-portada/PortadaSLOTS.png)


<a id="1-introduccion"></a>
## 1. Introducción
En este reto hablaremos sobre los distintos conectores que forman parte de un PC, especificaremos sus características y funciones y haremos distinciones entre conectores internos,externos y slots de expansión.

<a id="2-conectores-internos-energia"></a>
## 2. Conectores internos (energía)
# 12VHPWR / 12V-2x6 (PCIe 5.0 Power)
# 🧩 Función principal
Conector de nueva generación para tarjetas gráficas de alta potencia, diseñado para reemplazar múltiples conectores PCIe de 8 pines con una solución única de hasta 600W, introducido con PCIe 5.0 y mejorado en PCIe 5.1.​
# ⚙️ Características técnicas clave
12VHPWR (PCIe 5.0): Conector de 16 pines marcado con "H+"​

12V-2x6 (PCIe 5.1): Versión mejorada marcada con "H++", depreca al 12VHPWR​

Capacidad de potencia: Hasta 600W (55A @ 12V)​

Configuración de pines: 12 pines de potencia (+12V y GND) + 4 pines sideband (sense)​

Mejora principal del 12V-2x6: Pines de potencia 0.25mm más largos, pines sense 0.1mm más cortos para evitar conexión parcial y problemas de sobrecalentamiento​

Calibre de cable: 16AWG para aplicaciones de 600W​

Codificación: Puerto sideband más ancho en 12V-2x6 facilita inserción correcta​

# 🔌 Usos comunes
GPUs de última generación de NVIDIA (serie RTX 40 y 50) y próximas generaciones de AMD. Reemplaza configuraciones de 3x8 pines o 4x8 pines con un solo conector más compacto. Muchas PSUs incluyen adaptadores de 2x8 pines PCIe a 12VHPWR para compatibilidad.​
# 🏷️ Fuentes oficiales consultadas
Corsair 12VHPWR Technical Guide ( https://www.corsair.com/explorer/diy-builder/power-supply-units/evolving-standards-12vhpwr-and-12v-2x6/) 
​

Wikipedia - 12VHPWR ( https://es.wikipedia.org/wiki/12VHPWR )

# Fotografía
![12VHPWR](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/10-conectores_internos/12VHPWR%20-%2012V-2x6.jpg)

# ATX 24 pines (Main Power Connector)

# 🧩 Función principal
Conector principal de alimentación que suministra energía desde la fuente de alimentación (PSU) a la placa base, distribuyendo múltiples voltajes (+3.3V, +5V, +12V, -12V, +5VSB) a todos los componentes del sistema.​
# ⚙️ Características técnicas clave
Voltajes suministrados: +3.3V, +5V, +12V, -12V (opcional desde ATX 2.0), +5VSB (standby)

Capacidad de potencia: Hasta 300W+ (mejora respecto a los 250W del conector de 20 pines)​

Pinout: 24 pines con contactos Molex Mini-Fit Jr., pitch de 4.2mm​

Señales de control: PS_ON# (pin 16) para encendido, PWR_OK (pin 8) para indicación de voltaje estable​

Estándar: Introducido en ATX12V 2.0 (2003), especificación actual ATX 3.x​

Calibre de cable: Típicamente 18AWG para conductores de potencia​
# 🔌 Usos comunes
Alimentación esencial de la placa base en todos los PC de escritorio modernos. Proporciona energía a circuitos lógicos, memoria, slots PCIe, y gestión de energía del sistema. Compatible retroactivamente con conectores de 20 pines mediante adaptadores.​
# 🏷️ Fuentes oficiales consultadas
- Especificación oficial del estándar ATX desarrollado por Intel​ ( https://edc.intel.com/content/www/us/en/design/ipla/software-development-platforms/client/platforms/alder-lake-desktop/atx-version-3-0-multi-rail-desktop-platform-power-supply-design-guide/ )

- Seasonic PSU Technical Documentation ( https://seasonic.com/insights/seasonic-psu-cables/ )
  
- Especificaciones técnicas de implementación del conector ATX 24 pines​
eTechnophiles ATX Pinout Guide (https://www.etechnophiles.com/atx-power-supply-connector-pinout/ ) 

## Fotos
![Conector ATX 24 pines](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/10-conectores_internos/ATX24pines.jpg)

# EPS 8 pines (12V CPU Power)

# 🧩 Función principal
Conector dedicado de alimentación de 12V para el procesador (CPU), suministrando energía directa a los módulos reguladores de voltaje (VRM) de la placa base que alimentan el procesador.​
# ⚙️ Características técnicas clave
Voltaje: Exclusivamente +12V DC

Capacidad de potencia: Hasta 384W por conector de 8 pines​

Configuración: 8 pines (4+4 divisible), o 8+4 pines en placas de alto rendimiento, o 8+8 pines para overclocking extremo​

Calibre de cable: Típicamente 18AWG de cobre estañado​

Diferenciación física: Los pines tienen forma cuadrada distintiva para evitar confusión con conectores PCIe​

Estándar: ATX12V (evolución del conector de 4 pines original)​

# 🔌 Usos comunes
Alimentación dedicada para CPUs de escritorio de alto consumo. Los procesadores modernos de gama alta (Intel Core i9, AMD Ryzen 9) requieren estos conectores para operación estable. Configuraciones 8+4 o 8+8 permiten overclocking y suavizan las variaciones de voltaje.​
# 🏷️ Fuentes oficiales consultadas

ASRock Technical Wiki ( https://botflakes.de/asrockwiki/guides/whatIs12VEPS/ )

Exxact Technical Support ( https://support.exxactcorp.com/hc/en-us/articles/20180443940119 )

# Fotografía

![EPS8pines](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/10-conectores_internos/EPS%208%20pines.jpg)

# PCIe 6/8 pines (GPU Power)
# 🧩 Función principal
Conectores auxiliares de alimentación de 12V para tarjetas gráficas (GPUs) y otros dispositivos PCIe de alto consumo que requieren más potencia que los 75W proporcionados por el slot PCIe.​
# ⚙️ Características técnicas clave
Conector de 6 pines: Suministra hasta 75W según especificación PCI-SIG​

Conector de 8 pines (6+2): Suministra hasta 150W según especificación PCI-SIG​

Voltaje: +12V DC exclusivamente

Conductores reales: 6 conductores activos (3 para +12V, 3 para GND), los 2 pines adicionales en el conector de 8 pines son señales sense​

Capacidad real vs. especificación: Un cable bien construido puede manejar >300W, pero PCI-SIG limita a 150W para compatibilidad con PSUs de menor calidad​

Calibre de cable: Típicamente 18AWG, algunos de gama alta usan 16AWG​
# 🔌 Usos comunes
Alimentación de tarjetas gráficas dedicadas. GPUs modernas de gama media usan 1x8 pines, mientras que GPUs de alto rendimiento pueden requerir 2x8 pines o 3x8 pines. Ejemplo: RTX 4070 (1x8 pin), RTX 4080 (2x8 pines con adaptador).​
# 🏷️ Fuentes oficiales consultadas

Jon Gerow PCIe Analysis ( http://jongerow.com/PCIe/index.html )

Corsair GPU Power Guide ( https://www.corsair.com/us/en/explorer/diy-builder/power-supply-units/individual-8-pin-vs-pigtail-connectors-for-gpus/ ) 

# Fotografía
![PCIe 6a8 pines](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/10-conectores_internos/PCIe%206a8%20pines.jpg)

# SATA Power (15 pines)

# 🧩 Función principal
Conector de alimentación para dispositivos de almacenamiento SATA (discos duros, SSDs, unidades ópticas), proporcionando múltiples voltajes necesarios para la operación de estos dispositivos.​
# ⚙️ Características técnicas clave
Voltajes suministrados: +3.3V, +5V, +12V (3 pines por voltaje en paralelo para baja impedancia)​

Capacidad de corriente: 1.5A por pin, 4.5A total por voltaje​

Total de pines: 15 pines (5 para ground, 9 para voltajes, 1 opcional)​

Soporte hot-plug: Pines de diferentes longitudes permiten inserción/extracción en caliente​

Pin 3 (PWDIS): Definido en SATA 3.3 para modo de deshabilitación de energía, compatible con SAS​

Dimensiones: Conector de 1.27mm pitch, diseño wafer de 8mm de ancho​

# 🔌 Usos comunes
Alimentación estándar para discos duros SATA, SSDs de 2.5", unidades ópticas, y algunos dispositivos PCIe que requieren alimentación adicional. Compatible con adaptadores Molex de 4 pines, aunque el voltaje de 3.3V no estará disponible en ese caso.​

# 🏷️ Fuentes oficiales consultadas
Delkin SATA Technical Guide ( https://www.delkin.com/blog/sata-serial-ata/ )

Wikipedia - SATA ( https://es.wikipedia.org/wiki/Serial_ATA )

# Fotografía 
![SATA Power 15 pines](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/10-conectores_internos/SATA%20Power15pines.jpg)


<a id="3-conectores-de-datos"></a>
## 3. Conectores de datos

# SATA (Serial ATA)
# 🧩 Función principal
Interfaz de datos serial para conectar dispositivos de almacenamiento (HDDs, SSDs, unidades ópticas) a la placa base, reemplazando el antiguo estándar paralelo PATA/IDE.​
# ⚙️ Características técnicas clave
SATA 1.5 Gb/s (SATA Rev 1.x): Primera generación, hasta 150 MB/s efectivos​

SATA 3 Gb/s (SATA Rev 2.x): Segunda generación, hasta 300 MB/s efectivos​

SATA 6 Gb/s (SATA Rev 3.x): Tercera generación (actual), hasta 600 MB/s efectivos​

Conector de datos: 7 conductores (4 líneas de datos activas en 2 pares diferenciales, 3 grounds), conector wafer de 8mm​

Longitud de cable: Hasta 1 metro para SATA interno, hasta 2 metros para eSATA​

Codificación: 8b/10b encoding (80% de eficiencia)​

Características avanzadas: NCQ (Native Command Queuing), Hot-Plug, Staggered Spin-Up, Link Power Management​

# 🔌 Usos comunes
Conexión estándar de HDDs y SSDs SATA de 2.5" y 3.5" en PCs de escritorio y portátiles. Los SSDs SATA modernos alcanzan ~550 MB/s de lectura/escritura, cercano al límite teórico de SATA 6Gb/s. Siendo progresivamente reemplazado por NVMe para SSDs de alto rendimiento.​
# 🏷️ Fuentes oficiales consultadas
SATA-IO Official Website ( https://sata-io.org )

SATA-IO: Fast Just Got Faster White Paper ( https://sata-io.org/system/files/member-downloads/SATA-6Gbs-Fast-Just-Got-Faster_2.pdf ) - Documento oficial sobre SATA 6Gb/s​

SATA-IO Naming Guidelines ( https://sata-io.org/developers/sata-naming-guidelines ) - Convenciones oficiales de nomenclatura SATA​

# Fotografía
![SATA](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/11-conectores_datos/SATA.jpg)

# M.2 (NVMe / SATA)
# 🧩 Función principal
Factor de forma compacto y conector multi-protocolo que soporta SSDs de alto rendimiento usando interfaces PCIe (NVMe) o SATA, proporcionando velocidades significativamente superiores a SATA tradicional en el caso de NVMe.​
# ⚙️ Características técnicas clave
Conector: 75 posiciones con hasta 67 pines, pitch de 0.5mm, soporta hasta 50V y 0.5A por pin​

Keying (muescas):

Key B: SATA o PCIe x2 (hasta 2 lanes) - pines 12-19 sin contacto​

Key M: PCIe x4 (hasta 4 lanes) - pines 59-66 sin contacto​

Key B+M: Compatible con ambos slots, limitado a PCIe x2 o SATA​

Tamaños comunes: 2230, 2242, 2260, 2280, 22110 (ancho x largo en mm)​

Interfaces soportadas:

NVMe (PCIe): Hasta 4 lanes PCIe, velocidades de ~3500 MB/s (PCIe 3.0 x4) hasta ~14000 MB/s (PCIe 5.0 x4)​

SATA: Limitado a ~600 MB/s (mismo límite que SATA tradicional)​

Espesor de componentes: 1.5mm máximo por lado (varía según tipo)​

# 🔌 Usos comunes
SSDs NVMe M.2 son el estándar actual para almacenamiento de alto rendimiento en PCs de escritorio y portátiles. SSDs SATA M.2 se usan en sistemas más antiguos o configuraciones de presupuesto. Es crítico verificar el keying y protocolo soportado por el slot antes de comprar.​
# 🏷️ Fuentes oficiales consultadas
Wikipedia - M.2 ( https://es.wikipedia.org/wiki/M.2 ) 

Delock M.2 Interface Guide ( https://www.delock.com/infothek/M.2_2022/M.2_e.html )

Kingston M.2 vs SSD Guide ( https://www.kingston.com/en/blog/pc-performance/two-types-m2-vs-ssd )

# Fotografía 
![M2](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/11-conectores_datos/M.2%20(NVMe%20-%20SATA).jpg)


<a id="4-slots-de-expansion"></a>
## 4. Slots de expansión

# PCIe x1 / x4 / x8 / x16
# 🧩 Función principal
Slots de expansión serial de alto rendimiento para conectar tarjetas gráficas, SSDs NVMe, tarjetas de red, capturadoras de video y otros dispositivos de expansión, proporcionando bandwidth escalable según el número de lanes.​
# ⚙️ Características técnicas clave
Generaciones y Bandwidth (unidireccional por lane):

PCIe 3.0: 8 GT/s, ~985 MB/s por lane​

PCIe 4.0: 16 GT/s, ~1.969 GB/s por lane​

PCIe 5.0: 32 GT/s, ~3.938 GB/s por lane​

PCIe 6.0: 64 GT/s (en desarrollo)​

Bandwidth total por configuración (bidireccional):

x1: Hasta 2 GB/s (Gen 4), 4 GB/s (Gen 5)​

x4: Hasta 16 GB/s (Gen 4), 32 GB/s (Gen 5)​

x8: Hasta 32 GB/s (Gen 4), 64 GB/s (Gen 5)​

x16: Hasta 64 GB/s (Gen 4), 128 GB/s (Gen 5)​

Suministro de potencia por el slot:

x1: Hasta 10W (0.5A @ +12V + otros voltajes)​

x4/x8/x16: Hasta 75W (25W inicial, hasta 75W tras negociación)​

Compatibilidad física: Tarjetas más pequeñas funcionan en slots más grandes (ej: x1 en x16). Tarjetas más grandes en slots pequeños solo si el slot tiene extremo abierto.​​

# 🔌 Usos comunes
x1: Tarjetas WiFi, tarjetas de sonido, controladoras USB/SATA adicionales

x4: SSDs NVMe M.2 (vía adaptador), tarjetas de red 10GbE

x8: Tarjetas capturadoras de video, algunas GPUs de gama media

x16: Tarjetas gráficas dedicadas (GPUs), el slot primario suele ser el único cableado a x16 completo​​

# 🏷️ Fuentes oficiales consultadas
PCI-SIG Official Specifications (https://pcisig.com/specifications)

Trenton Systems PCIe 4.0 Guide (https://www.trentonsystems.com/en-us/resource-hub/blog/pcie-gen-4-reference-guide)

Gamers Nexus PCIe 5.0 Testing (https://gamersnexus.net/gpus/nvidia-rtx-5090-pcie-50-vs-40-vs-30-x16-scaling-benchmarks) - Testing técnico de diferencias entre generaciones PCIe​

Wikipedia - PCI Express (https://es.wikipedia.org/wiki/PCI_Express)

# Fotografía

![PCIe](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/12-slots_expansion/PCIe%20x1%20-%20x4%20-%20x8%20-%20x16.jpg)

# M.2 slot para WiFi / Bluetooth (Key E / Key A+E)
# 🧩 Función principal
Slot M.2 especializado en placas base para módulos de conectividad inalámbrica (WiFi, Bluetooth, WWAN), utilizando keying específico (Key E o A+E) y típicamente con soporte para 1-2 lanes PCIe.​
# ⚙️ Características técnicas clave
Key E: Pines 24-31 sin contacto, soporta 2x PCIe x1, USB 2.0, I²C, SDIO, UART, PCM y CNVi​

Key A+E: Combinación de pines 8-15 y 24-31 sin contacto, soporta 2x PCIe x1, USB 2.0 y CNVi​

Tamaños soportados: Típicamente 2230 (más común para WiFi), 1630, 3030​

Interfaces soportadas: PCIe (para WiFi), USB 2.0 (para Bluetooth), CNVi (WiFi integrado Intel)​

Conexiones adicionales: Suele incluir conectores U.FL o MHF4 para antenas externas​

Montaje: Tornillo de fijación en posición 2230, componentes máximo 1.2-1.5mm de altura​

# 🔌 Usos comunes
Módulos WiFi 6/6E/7 y Bluetooth 5.x en placas base de escritorio. Módulos comunes incluyen Intel AX210, AX211 (CNVi), MediaTek MT7922. Permite actualizar conectividad inalámbrica sin ocupar slots PCIe estándar. Algunas placas incluyen el módulo preinstalado ("WiFi integrado").​
# 🏷️ Fuentes oficiales consultadas
Wikipedia - M.2 (https://es.wikipedia.org/wiki/M.2) - Tabla de keying oficial con interfaces soportadas por Key E y A+E​

Newegg M.2 WiFi Adapter Listing ( https://www.newegg.ca/p/1B0-01B8-000C0 ) - Especificaciones de adaptadores M.2 Key E​

# Fotografía
![M.2WiFi](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/12-slots_expansion/M.2%20slot%20para%20WiFi%20-%20Bluetooth%20.jpg)



<a id="5-conectores-externos"></a>
## 5. Conectores externos

# USB-A 2.0 / 3.x
# 🧩 Función principal
Conector rectangular estándar tradicional para periféricos USB, con múltiples generaciones que proporcionan diferentes velocidades de transferencia desde 480 Mbps (USB 2.0) hasta 20 Gbps (USB 3.2 Gen 2x2).​
# ⚙️ Características técnicas clave
Generaciones USB-A:

USB 2.0 (Negro): Hasta 480 Mbps, 5V @ 0.5A (2.5W)​

USB 3.2 Gen 1 / "SuperSpeed USB 5Gbps" (Azul): Hasta 5 Gbps, 5V @ 0.9A (4.5W)​

USB 3.2 Gen 2 / "SuperSpeed USB 10Gbps" (Azul o teal): Hasta 10 Gbps, 5V @ 0.9A​

USB 3.2 Gen 2x2 / "SuperSpeed USB 20Gbps": Hasta 20 Gbps (requiere cable USB-C dual-lane)​

Dimensiones del conector Type-A:

Receptáculo interno: 12.35mm ancho x 4.5mm alto x 15.2mm profundo​

Plug externo: 11.5mm ancho x 4.0mm alto x 14.5mm largo​

Codificación:

USB 2.0 y USB 3.2 Gen 1: 8b/10b (80% eficiencia)​

USB 3.2 Gen 2 y superiores: 128b/132b (96.97% eficiencia)​

# 🔌 Usos comunes
Periféricos de PC estándar: teclados, ratones, memorias USB, discos duros externos, impresoras. USB 2.0 (negro) suficiente para periféricos de baja velocidad. USB 3.x (azul) necesario para almacenamiento externo rápido. Siendo gradualmente reemplazado por USB-C en dispositivos nuevos.​
# 🏷️ Fuentes oficiales consultadas
Wikipedia - USB 3.0 (https://es.wikipedia.org/wiki/USB_3.0)

USB-IF USB 3.2 Specification (https://www.usb.org/usb-32-0) - Especificación oficial USB 3.2 del USB Implementers Forum​

Wikipedia - USB Hardware (https://es.wikipedia.org/wiki/USB_hardware) - Dimensiones oficiales de conectores USB​

# Fotografía

![USBa2.0](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/Usb%202.0%20y%203.0.png)

# USB-B
# 🧩 Función principal
Conector cuadrado/rectangular usado en el lado del dispositivo (device-side) para prevenir conexiones incorrectas host-to-host, principalmente en impresoras, escáneres y cámaras PTZ.​
# ⚙️ Características técnicas clave
USB 2.0 Type-B (Negro):

Velocidad: Hasta 480 Mbps​

Potencia: 5V @ 0.5A (2.5W)​

Dimensiones receptáculo: 11.1mm ancho x 7.0mm alto x 12.0mm profundo​

Pines: 4 pines (VBUS, D-, D+, GND)​

USB 3.0 Type-B (Azul):

Velocidad: Hasta 5 Gbps​

Potencia: 5V @ 0.9A (4.5W)​

Forma física: Extensión superior añadida al conector 2.0 para pines adicionales SuperSpeed​

Compatibilidad: Plugs USB 2.0 Type-B caben en receptáculos 3.0, pero no viceversa​

Variantes:
Mini-B: 7.5mm x 3.0mm, usado en cámaras y dispositivos antiguos (deprecated)​

Micro-B: 6.85mm x 1.8mm, usado en smartphones Android antiguos​

# 🔌 Usos comunes
Impresoras USB (casi todas usan Type-B estándar), escáneres, interfaces de audio profesionales, cámaras PTZ para videoconferencia. El diseño previene que dos hosts se conecten accidentalmente, lo cual podría causar daño al hardware.​

# 🏷️ Fuentes oficiales consultadas

CMD USB Identification Guide (https://www.cmd-ltd.com/advice-centre/usb-chargers-and-power-modules/usb-and-power-module-product-help/identifying-usb-connector/)ç

Wikipedia - USB Hardware (https://es.wikipedia.org/wiki/USB_hardware) 

# Fotografía

![USBb](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/UsbB.jpg)

# USB-C / USB4
# 🧩 Función principal
Conector reversible de última generación que unifica transferencia de datos de alta velocidad, video (DisplayPort Alt Mode), y carga de alta potencia (hasta 240W) en un solo puerto, con USB4 alcanzando hasta 80 Gbps.​
# ⚙️ Características técnicas clave
USB4 Gen 2x2 (20 Gbps): Velocidad mínima obligatoria para USB4​

USB4 Gen 3x2 (40 Gbps): Velocidad estándar USB4, equivalente a Thunderbolt 3​

USB4 Gen 4 (80 Gbps): Versión 2.0 del estándar USB4, usando codificación PAM3​

USB Power Delivery: Hasta 240W (48V @ 5A) según especificación USB PD 3.1​

Protocolo tunneling: Multiplexación de USB, DisplayPort y PCIe sobre el mismo cable​

Compatibilidad: Full backward compatibility con USB 3.2, USB 2.0, y Thunderbolt 3/4​

DisplayPort Alt Mode: Hasta 8K @ 60Hz o 4K @ 144Hz sobre USB-C​

Longitud de cable: Hasta 2 metros para 40 Gbps, hasta 1 metro para 80 Gbps pasivo​

# 🔌 Usos comunes

Puerto universal en laptops y dispositivos móviles modernos para carga, transferencia de datos, y conexión de displays. Usado en docks USB4/Thunderbolt, SSDs externos de alta velocidad, y conexión directa de monitores. Reemplaza progresivamente todos los puertos legacy (USB-A, HDMI, DisplayPort).​
# 🏷️ Fuentes oficiales consultadas

USB-IF Official USB4 Page (https://www.usb.org/usb4) - Especificaciones oficiales del USB4

USB-IF USB4 V2.0 Release (https://www.eetasia.com/usb-if-releases-usb4-specs/) - Anuncio oficial de USB4 80Gbps​

# Fotografía

![USBc-4](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/USB-C%20-%20USB4.jpg)

# HDMI 2.1
# 🧩 Función principal
Interfaz de video y audio digital de alta definición, con HDMI 2.1 proporcionando bandwidth suficiente para 8K@60Hz, 4K@120Hz y funciones avanzadas como VRR y eARC para gaming y home theater.​
# ⚙️ Características técnicas clave
Bandwidth total: 48 Gbps (4 lanes @ 12 Gbit/s cada uno)​

Data rate efectivo: ~42.6 Gbps (codificación 16b/18b, 88.8% eficiencia)​

Resoluciones soportadas:

10K @ 120Hz (con DSC)

8K @ 60Hz (sin compresión, 8bpc RGB/YCbCr 4:4:4)​

4K @ 120Hz (sin compresión)​

Features avanzados:

VRR (Variable Refresh Rate): Eliminación de screen tearing para gaming​

eARC (Enhanced Audio Return Channel): Soporte para audio objeto como Dolby Atmos y DTS:X​

QFT (Quick Frame Transport): Reducción de latencia​

ALLM (Auto Low Latency Mode): Conmutación automática a modo gaming​

Dynamic HDR: Metadatos HDR por escena o frame​

HDMI 2.1a: Añade Source-Based Tone Mapping (2022)​

HDMI 2.2 (anunciado enero 2025, lanzado junio 2025): Bandwidth hasta 96 Gbps​

# 🔌 Usos comunes
Conexión de GPUs modernas a monitores gaming 4K@120Hz+ o TVs 8K. Consolas PlayStation 5 y Xbox Series X requieren HDMI 2.1 para aprovechar 4K@120Hz. Home theater para audio Dolby Atmos/DTS:X vía eARC.​

# 🏷️ Fuentes oficiales consultadas
Wikipedia - HDMI (https://es.wikipedia.org/wiki/HDMI) - Especificaciones técnicas oficiales HDMI 2.1 y 2.2​

HDMI Forum Press Release (https://www.hdmi.org/download/pressfileid/60) - Anuncio oficial de HDMI 2.1 con especificaciones​

# Fotografía

![HDMI2.1](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/HDMI%202.1%20.jpg)

# DisplayPort 1.4 / 2.1
# 🧩 Función principal
Interfaz de video digital de alto rendimiento desarrollada por VESA, con DisplayPort 2.1 proporcionando hasta 80 Gbps de bandwidth para resoluciones y refresh rates extremos, superando significativamente a HDMI.​
# ⚙️ Características técnicas clave
DisplayPort 1.4 (HBR3):

Bandwidth: 32.4 Gbps bruto (25.92 Gbps efectivo, codificación 8b/10b, 80% eficiencia)​

Resoluciones: 8K @ 30Hz, 4K @ 120Hz (ambos con DSC), 4K @ 60Hz sin compresión​

DisplayPort 2.1 (UHBR):

Bandwidth máximo: 80 Gbps (UHBR20), 77.37 Gbps efectivo (codificación 128b/132b, 96.7% eficiencia)​

Modos UHBR:

UHBR10: 40 Gbps (38.69 Gbps efectivo)​

UHBR13.5: 54 Gbps (52.22 Gbps efectivo)​

UHBR20: 80 Gbps (77.37 Gbps efectivo)​

Resoluciones sin compresión: 10K @ 60Hz, 4K @ 240Hz, 8K @ 60Hz​

Resoluciones con DSC: 16K @ 60Hz, 8K @ 120Hz​

Certificación de cables:

DP40: Soporta hasta UHBR10 (40 Gbps), cables hasta 2 metros​

DP80: Soporta hasta UHBR20 (80 Gbps), cables hasta 1 metro​

Features adicionales:

DSC (Display Stream Compression): Compresión visualmente lossless, obligatorio en DP 2.1​

Panel Replay: Reduce bandwidth en >99% cuando no hay cambios en pantalla​

DisplayPort Alt Mode: Funciona sobre USB-C​

Multi-Stream Transport (MST): Daisy-chaining de múltiples monitores​

# 🔌 Usos comunes
Monitores gaming de alta velocidad (4K@240Hz, 1440p@360Hz+), monitores profesionales 8K, configuraciones multi-monitor vía MST. DisplayPort 2.1 actualmente limitado a GPUs AMD RX 7000 y algunos monitores premium, pero se espera adopción más amplia en 2025-2026.​

# 🏷️ Fuentes oficiales consultadas
VESA DisplayPort 2.1 Release (https://vesa.org/featured-articles/vesa-releases-displayport-2-1-specification/) - Anuncio oficial de DisplayPort 2.1 por VESA​

DisplayNinja DP 2.1 Guide (https://www.displayninja.com/what-is-displayport-2-1/) - Análisis técnico detallado con especificaciones VESA​

# Fotografía 

![DP2.1vs1.4](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/DP2.1%20vs%201.4.jpg)


# RJ45 Ethernet (1G / 2.5G / 10G)
# 🧩 Función principal
Conector modular de 8 pines para redes Ethernet cableadas, proporcionando conexión confiable de baja latencia con velocidades desde 1 Gigabit hasta 10 Gigabits por segundo, soportado por múltiples estándares IEEE 802.3.​
# ⚙️ Características técnicas clave
1 Gigabit Ethernet (1GbE / 1000BASE-T):

Velocidad: Hasta 1 Gbps (~125 MB/s)​
Estándar: IEEE 802.3ab​
Cableado: Cat5e o superior, hasta 100 metros​
Latencia: Media​

2.5 Gigabit Ethernet (2.5GbE / 2.5GBASE-T):

Velocidad: Hasta 2.5 Gbps (~312.5 MB/s), 2.5x más rápido que 1GbE​
Estándar: IEEE 802.3bz (2016)​
Cableado: Cat5e o superior, hasta 100 metros (ventaja clave vs 10GbE)​
Compatibilidad: Auto-negotiation con 1GbE y 10GbE​
Uso: Ideal para aprovechar WiFi 6/6E/7 (>1Gbps) sin rewiring​

10 Gigabit Ethernet (10GbE / 10GBASE-T):

Velocidad: Hasta 10 Gbps (~1.25 GB/s)​
Estándares: IEEE 802.3an (10GBASE-T)​
Cableado: Cat6a hasta 100 metros, Cat6 hasta ~55 metros​
Consumo: Mayor que 1GbE/2.5GbE​
Uso: Entornos profesionales, datacenters, workstations con almacenamiento NAS de alto rendimiento​

Variantes adicionales (NBASE-T):

5GBASE-T: 5 Gbps, sobre Cat5e/Cat6​
# 🔌 Usos comunes
1GbE: Estándar para PCs domésticos y oficina, suficiente para navegación, streaming 4K y gaming online.

2.5GbE: Creciente adopción en motherboards gaming/entusiasta 2023-2025, ideal para aprovechar WiFi 6 y NAS de alta velocidad sin cambiar cableado.

10GbE: Workstations profesionales, servidores, edición de video 4K/8K desde NAS, entornos virtualizados.​

# 🏷️ Fuentes oficiales consultadas
VSOL 2.5GbE Overview ( https://www.vsolcn.com/blog/25-gigabit-ethernet-25gbe-overview.html ) - Guía técnica de 2.5GbE según IEEE 802.3bz​

Lucid 10G Ethernet Card Specs ( https://thinklucid.com/product/10g-5g-2-5g-1g-poe-ethernet-card/ ) - Especificaciones de implementación NBASE-T​

# Fotografía

![RJ45](/retos/Reto_01_Investigacion_Desarrollo_Conectores_Slots/assets/img/20-conectores_externos/cable-RJ45%20tipos.jpg)



<a id="6-bibliografia"></a>
## 6. Bibliografía

Aquí todas las fuentes consultadas para la realización de este reto: 
# 🏷️ Fuentes oficiales consultadas
12VHPWR:
Corsair 12VHPWR Technical Guide ( https://www.corsair.com/explorer/diy-builder/power-supply-units/evolving-standards-12vhpwr-and-12v-2x6/) 
​

Wikipedia - 12VHPWR ( https://es.wikipedia.org/wiki/12VHPWR )
ATX:
- Especificación oficial del estándar ATX desarrollado por Intel​ ( https://edc.intel.com/content/www/us/en/design/ipla/software-development-platforms/client/platforms/alder-lake-desktop/atx-version-3-0-multi-rail-desktop-platform-power-supply-design-guide/ )

- Seasonic PSU Technical Documentation ( https://seasonic.com/insights/seasonic-psu-cables/ )
  
- Especificaciones técnicas de implementación del conector ATX 24 pines​
eTechnophiles ATX Pinout Guide (https://www.etechnophiles.com/atx-power-supply-connector-pinout/ )
EPS:
ASRock Technical Wiki ( https://botflakes.de/asrockwiki/guides/whatIs12VEPS/ )

Exxact Technical Support ( https://support.exxactcorp.com/hc/en-us/articles/20180443940119 )

PCIe6-8pines: 
Jon Gerow PCIe Analysis ( http://jongerow.com/PCIe/index.html )

Corsair GPU Power Guide ( https://www.corsair.com/us/en/explorer/diy-builder/power-supply-units/individual-8-pin-vs-pigtail-connectors-for-gpus/ ) 

SATA Power:
Delkin SATA Technical Guide ( https://www.delkin.com/blog/sata-serial-ata/ )

Wikipedia - SATA ( https://es.wikipedia.org/wiki/Serial_ATA )

SATA:
SATA-IO Official Website ( https://sata-io.org )

SATA-IO: Fast Just Got Faster White Paper ( https://sata-io.org/system/files/member-downloads/SATA-6Gbs-Fast-Just-Got-Faster_2.pdf ) - Documento oficial sobre SATA 6Gb/s​

SATA-IO Naming Guidelines ( https://sata-io.org/developers/sata-naming-guidelines ) - Convenciones oficiales de nomenclatura SATA​

M2:
Wikipedia - M.2 ( https://es.wikipedia.org/wiki/M.2 ) 

Delock M.2 Interface Guide ( https://www.delock.com/infothek/M.2_2022/M.2_e.html )

Kingston M.2 vs SSD Guide ( https://www.kingston.com/en/blog/pc-performance/two-types-m2-vs-ssd )

M2WiFi:
Wikipedia - M.2 (https://es.wikipedia.org/wiki/M.2) - Tabla de keying oficial con interfaces soportadas por Key E y A+E​

Newegg M.2 WiFi Adapter Listing ( https://www.newegg.ca/p/1B0-01B8-000C0 ) - Especificaciones de adaptadores M.2 Key E​

PCIe x1 x4 x8 x16:
PCI-SIG Official Specifications (https://pcisig.com/specifications)

Trenton Systems PCIe 4.0 Guide (https://www.trentonsystems.com/en-us/resource-hub/blog/pcie-gen-4-reference-guide)

Gamers Nexus PCIe 5.0 Testing (https://gamersnexus.net/gpus/nvidia-rtx-5090-pcie-50-vs-40-vs-30-x16-scaling-benchmarks) - Testing técnico de diferencias entre generaciones PCIe​

Wikipedia - PCI Express (https://es.wikipedia.org/wiki/PCI_Express)

USB A:
Wikipedia - USB 3.0 (https://es.wikipedia.org/wiki/USB_3.0)

USB-IF USB 3.2 Specification (https://www.usb.org/usb-32-0) - Especificación oficial USB 3.2 del USB Implementers Forum​

Wikipedia - USB Hardware (https://es.wikipedia.org/wiki/USB_hardware) - Dimensiones oficiales de conectores USB​

USB B:
CMD USB Identification Guide (https://www.cmd-ltd.com/advice-centre/usb-chargers-and-power-modules/usb-and-power-module-product-help/identifying-usb-connector/)ç

Wikipedia - USB Hardware (https://es.wikipedia.org/wiki/USB_hardware) 

USB C:
USB-IF Official USB4 Page (https://www.usb.org/usb4) - Especificaciones oficiales del USB4

USB-IF USB4 V2.0 Release (https://www.eetasia.com/usb-if-releases-usb4-specs/) - Anuncio oficial de USB4 80Gbps​

HDMI2.1:
Wikipedia - HDMI (https://es.wikipedia.org/wiki/HDMI) - Especificaciones técnicas oficiales HDMI 2.1 y 2.2​

HDMI Forum Press Release (https://www.hdmi.org/download/pressfileid/60) - Anuncio oficial de HDMI 2.1 con especificaciones​

DP 1.4-2.1:
VESA DisplayPort 2.1 Release (https://vesa.org/featured-articles/vesa-releases-displayport-2-1-specification/) - Anuncio oficial de DisplayPort 2.1 por VESA​

DisplayNinja DP 2.1 Guide (https://www.displayninja.com/what-is-displayport-2-1/) - Análisis técnico detallado con especificaciones VESA​

RJ45:
VSOL 2.5GbE Overview ( https://www.vsolcn.com/blog/25-gigabit-ethernet-25gbe-overview.html ) - Guía técnica de 2.5GbE según IEEE 802.3bz​

Lucid 10G Ethernet Card Specs ( https://thinklucid.com/product/10g-5g-2-5g-1g-poe-ethernet-card/ ) - Especificaciones de implementación NBASE-T​

# Conceptos Básicos de Redes y Ciberseguridad
2
 
3
## ¿Qué es una Red?
4
 
5
Una red es un conjunto de dispositivos conectados entre sí que intercambian información y recursos.
6
 
7
### Ejemplos de dispositivos
8
 
9
- Computadores
10
- Servidores
11
- Switches
12
- Routers
13
- Impresoras
14
- Smartphones
15
 
16
### Tipos de red
17
 
18
| Tipo | Descripción |
19
|--------|------------|
20
| PAN | Red personal |
21
| LAN | Red local |
22
| MAN | Red metropolitana |
23
| WAN | Red de área amplia |
24
| WLAN | Red inalámbrica |
25
 
26
---
27
 
28
# ¿Qué es Internet?
29
 
30
Internet es una red mundial compuesta por millones de dispositivos conectados mediante el conjunto de protocolos TCP/IP.
31
 
32
Características:
33
 
34
- Descentralizada
35
- Escalable
36
- Global
37
- Basada en estándares
38
 
39
---
40
 
41
# Host
42
 
43
Un host es cualquier dispositivo conectado a una red con capacidad para enviar y recibir datos.
44
 
45
Ejemplos:
46
 
47
- PC
48
- Laptop
49
- Servidor
50
- Smartphone
51
- Cámara IP
52
 
53
---
54
 
55
# Dirección IP
56
 
57
Una dirección IP identifica de forma lógica a un dispositivo dentro de una red.
58
 
59
Ejemplo IPv4:
60
 
61
```text
62
192.168.1.10
63
```
64
 
65
Ejemplo IPv6:
66
 
67
```text
68
2001:db8::1
69
```
70
 
71
---
72
 
73
# Dirección MAC
74
 
75
Una dirección MAC es un identificador físico único asignado a una interfaz de red.
76
 
77
Ejemplo:
78
 
79
```text
80
00:1A:2B:3C:4D:5E
81
```
82
 
83
Características:
84
 
85
- 48 bits
86
- Única por fabricante
87
- Opera en Capa 2
88
 
89
---
90
 
91
# Router
92
 
93
Dispositivo que conecta diferentes redes y dirige los paquetes de datos.
94
 
95
Funciones:
96
 
97
- Enrutamiento
98
- Conexión a Internet
99
- NAT
100
- Seguridad básica
101
 
102
---
103
 
104
# Switch
105
 
106
Dispositivo que conecta equipos dentro de una misma red.
107
 
108
Funciones:
109
 
110
- Aprender direcciones MAC
111
- Reenviar tráfico eficientemente
112
- Segmentar dominios de colisión
113
 
114
---
115
 
116
# Hub
117
 
118
Dispositivo antiguo que replica el tráfico a todos los puertos.
119
 
120
Desventajas:
121
 
122
- Bajo rendimiento
123
- Sin inteligencia de red
124
- Poco seguro
125
 
126
---
127
 
128
# Cliente y Servidor
129
 
130
## Cliente
131
 
132
Equipo que solicita servicios.
133
 
134
Ejemplo:
135
 
136
- Navegador web
137
 
138
## Servidor
139
 
140
Equipo que entrega servicios.
141
 
142
Ejemplos:
143
 
144
- Servidor Web
145
- Servidor DNS
146
- Servidor DHCP
147
 
148
---
149
 
150
# Paquete
151
 
152
Unidad de información transmitida a través de una red.
153
 
154
Un paquete contiene:
155
 
156
- Dirección origen
157
- Dirección destino
158
- Datos
159
- Información de control
160
 
161
---
162
 
163
# Puerto
164
 
165
Número lógico utilizado para identificar servicios o aplicaciones.
166
 
167
Ejemplos:
168
 
169
| Puerto | Servicio |
170
|----------|----------|
171
| 22 | SSH |
172
| 53 | DNS |
173
| 80 | HTTP |
174
| 443 | HTTPS |
175
 
176
---
177
 
178
# Protocolo
179
 
180
Conjunto de reglas que permiten la comunicación entre dispositivos.
181
 
182
Ejemplos:
183
 
184
- TCP
185
- UDP
186
- HTTP
187
- HTTPS
188
- DNS
189
- DHCP
190
 
191
---
192
 
193
# Ancho de Banda
194
 
195
Cantidad máxima de datos que pueden transmitirse en un tiempo determinado.
196
 
197
Medidas comunes:
198
 
199
```text
200
Mbps
201
Gbps
202
Tbps
203
```
204
 
205
---
206
 
207
# Latencia
208
 
209
Tiempo que tarda un paquete en viajar desde el origen hasta el destino.
210
 
211
Generalmente se mide en:
212
 
213
```text
214
Milisegundos (ms)
215
```
216
 
217
---
218
 
219
# DNS
220
 
221
Domain Name System.
222
 
223
Convierte nombres de dominio en direcciones IP.
224
 
225
Ejemplo:
226
 
227
```text
228
google.com → 142.250.x.x
229
```
230
 
231
---
232
 
233
# DHCP
234
 
235
Dynamic Host Configuration Protocol.
236
 
237
Asigna automáticamente:
238
 
239
- Dirección IP
240
- Máscara de red
241
- Gateway
242
- DNS
243
 
244
---
245
 
246
# Gateway
247
 
248
Puerta de enlace utilizada para salir de una red local hacia otras redes.
249
 
250
Ejemplo:
251
 
252
```text
253
192.168.1.1
254
```
255
 
256
---
257
 
258
# VPN
259
 
260
Virtual Private Network.
261
 
262
Permite crear una conexión segura y cifrada a través de Internet.
263
 
264
Beneficios:
265
 
266
- Privacidad
267
- Protección de datos
268
- Acceso remoto seguro
269
 
270
---
271
 
272
# Firewall
273
 
274
Sistema de seguridad que controla el tráfico de red.
275
 
276
Funciones:
277
 
278
- Permitir conexiones
279
- Bloquear conexiones
280
- Registrar eventos
281
 
282
Ejemplos:
283
 
284
- Windows Firewall
285
- pfSense
286
- Fortinet
287
- Palo Alto
288
 
289
---
290
 
291
# Malware
292
 
293
Software diseñado para dañar o comprometer sistemas.
294
 
295
Tipos:
296
 
297
- Virus
298
- Gusanos
299
- Troyanos
300
- Spyware
301
- Ransomware
302
 
303
---
304
 
305
# Vulnerabilidad
306
 
307
Debilidad que puede ser explotada por una amenaza.
308
 
309
Ejemplos:
310
 
311
- Software desactualizado
312
- Contraseñas débiles
313
- Mala configuración
314
 
315
---
316
 
317
# Amenaza
318
 
319
Cualquier evento o actor capaz de explotar una vulnerabilidad.
320
 
321
Ejemplos:
322
 
323
- Hackers
324
- Malware
325
- Desastres naturales
326
- Error humano
327
 
328
---
329
 
330
# Riesgo
331
 
332
Probabilidad de que una amenaza explote una vulnerabilidad generando un impacto negativo.
333
 
334
Fórmula conceptual:
335
 
336
```text
337
Riesgo = Amenaza × Vulnerabilidad × Impacto
338
```
339
 
340
---
341
 
342
# Autenticación
343
 
344
Proceso para verificar la identidad de un usuario.
345
 
346
Factores:
347
 
348
### Algo que sé
349
 
350
- Contraseña
351
- PIN
352
 
353
### Algo que tengo
354
 
355
- Token
356
- Smartphone
357
 
358
### Algo que soy
359
 
360
- Huella digital
361
- Reconocimiento facial
362
 
363
---
364
 
365
# Principio de Mínimo Privilegio
366
 
367
Un usuario debe tener solamente los permisos necesarios para realizar su trabajo.
368
 
369
Beneficios:
370
 
371
- Reduce riesgos
372
- Limita ataques
373
- Mejora la seguridad
374
 
375
---
376
 
377
# Copia de Seguridad (Backup)
378
 
379
Proceso de creación de copias de datos para su recuperación ante incidentes.
380
 
381
Regla 3-2-1:
382
 
383
- 3 copias de los datos
384
- 2 medios distintos
385
- 1 copia fuera del sitio
386
 
387
---
388
 
389
# Conceptos Clave para Recordar
390
 
391
✅ IP identifica dispositivos.
392
 
393
✅ MAC identifica interfaces físicas.
394
 
395
✅ DNS traduce nombres a IP.
396
 
397
✅ DHCP asigna configuraciones automáticamente.
398
 
399
✅ Router conecta redes.
400
 
401
✅ Switch conecta dispositivos.
402
 
403
✅ Firewall filtra tráfico.
404
 
405
✅ Vulnerabilidad ≠ Amenaza.
406
 
407
✅ Riesgo = Amenaza + Vulnerabilidad + Impacto.
408
 
409
✅ La seguridad empieza por los principios básicos.

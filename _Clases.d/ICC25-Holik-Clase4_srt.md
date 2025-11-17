1
00:00:03,180 --> 00:00:08,380
Bueno, estamos grabando, como les decía, Leandro Batlle de Fundación Sadosky,

2
00:00:08,560 --> 00:00:16,139
cordialmente se ofreció para explicarles cómo instalar Python en sus computadoras y cómo

3
00:00:16,219 --> 00:00:21,620
poder correr algún archivito muy sencillo de Python. Es así, Leandro, cuando quieras,

4
00:00:21,700 --> 00:00:27,020
compartí pantalla y comenzá, por favor. Vamos, voy compartiendo, buen día a todos,

5
00:00:27,120 --> 00:00:38,540
a todos estoy compartiendo, entiendo que sí buenísimo bueno voy a tomar unos 10 minutos

6
00:00:39,760 --> 00:00:44,920
para comentar un poquito las opciones que tenemos para correr python y cuadernos Jupyter

7
00:00:47,260 --> 00:00:58,180
remoto en la nube como local y digamos voy a ir muy rápido en cuanto a las opciones que tenemos y

8
00:00:58,220 --> 00:01:04,220
después voy a explicar un poquito voy a mostrar un entorno Python y cuadernos Jupyter corriendo

9
00:01:04,280 --> 00:01:10,540
local en mi máquina. Bien, bueno, se ve, se escucha ¿no? ¿Voy bien?

10
00:01:12,439 --> 00:01:13,260
Sí, se acuerda.

11
00:01:13,960 --> 00:01:19,700
Claro, claro. Bueno, entonces, entonces arrancamos. Miren, esta, lo primero que quiero comentar

12
00:01:19,780 --> 00:01:28,979
es que tienen el código fuente disponible de esta presentación acá en este URL, si

13
00:01:28,980 --> 00:01:35,380
si lo quieren sacar de ahí, para así pueden copypastear cualquier cosa que vean durante

14
00:01:35,480 --> 00:01:48,740
la presentación. El URL es este que está acá, que es un repositorio Git. Miren, arrancamos

15
00:01:48,860 --> 00:01:55,140
con la, digamos, el árbol de decisión que tenemos acá. Primero, para compu cuántica.

16
00:01:57,980 --> 00:02:04,460
una cosa muy importante, ineludible en el proceso de trabajo de computación cuántica

17
00:02:04,460 --> 00:02:08,280
es la simulación. Uno piensa "bueno, pero si están las compu cuánticas reales...", bueno, no.

18
00:02:08,759 --> 00:02:14,900
Las compu cuánticas, si o si corren remoto, vía nube, ahí sí que no hay decisión,

19
00:02:15,600 --> 00:02:21,420
la decisión la tomaron por nosotros, pero para la simulación, dentro de la simulación,

20
00:02:22,660 --> 00:02:29,900
decir, amplío un poco eso. La mayoría de los SDKs de compu cuántica no te dejan correr,

21
00:02:29,990 --> 00:02:34,480
no te dejan acolar un trabajo en una compu cuántica física si antes no lo simulaste local.

22
00:02:35,920 --> 00:02:42,680
Ya sea con cualquiera de las, digamos, ocho combinaciones que tenemos de ahí para abajo

23
00:02:42,680 --> 00:02:48,739
en los tres renglones de abajo. Entonces, sí o sí vamos a tener que simular. Y para

24
00:02:48,740 --> 00:02:55,360
así, lo buena, la buena noticia es que para simular, no sé, 10 qubits hasta 20 qubits,

25
00:02:55,760 --> 00:03:01,680
más o menos con cualquier máquina estaríamos más o menos bien, con lo cual podemos tranquilamente

26
00:03:02,000 --> 00:03:08,540
de acá para abajo decidir con libertad si segundo ringlón vamos a correr la simulación

27
00:03:08,620 --> 00:03:17,139
local o en la nube. Por ejemplo, ejemplos de correr en la nube sería, por ejemplo, cuadernos 

28
00:03:17,140 --> 00:03:20,620
Jupyter disfrazados de Google Colab.

29
00:03:23,200 --> 00:03:25,920
Una vez que decidimos si lo corremos local,

30
00:03:26,220 --> 00:03:29,740
ahí está en negrita las decisiones de todo ese árbol de

31
00:03:29,780 --> 00:03:33,060
decisión, las decisiones que vamos a ilustrar hoy.

32
00:03:33,360 --> 00:03:35,400
Entonces, sí o sí lo vamos a simular,

33
00:03:35,600 --> 00:03:37,540
sí o sí lo vamos a simular en un entorno local.

34
00:03:38,980 --> 00:03:42,080
Y después, ¿qué entorno de Python vamos a usar?

35
00:03:42,300 --> 00:03:45,560
Ahí hay otra decisión que medio está implícita,

36
00:03:45,660 --> 00:03:47,920
que es que lo vamos a correr con el SDK de Python.

37
00:03:49,000 --> 00:03:51,080
No sé si hay realmente opciones a Python.

38
00:03:52,920 --> 00:03:55,060
Una vez que lo corremos con Python y local,

39
00:03:55,680 --> 00:03:56,460
¿qué vamos a usar?

40
00:03:56,660 --> 00:04:00,940
El entorno de Python del sistema operativo o un entorno

41
00:04:01,020 --> 00:04:01,500
virtual.

42
00:04:02,400 --> 00:04:04,940
Virtual, ahora sí, en el sentido informático de la

43
00:04:05,100 --> 00:04:05,420
palabra, ¿no?

44
00:04:05,540 --> 00:04:10,680
O sea, es un contexto aparte del Python de sistema operativo.

45
00:04:12,260 --> 00:04:16,400
Craso error, craso error toquetear el Python que viene con el sistema operativo,

46
00:04:16,600 --> 00:04:20,900
porque lo necesitan todas las aplicaciones de, digamos, de sistema, etcétera.

47
00:04:20,970 --> 00:04:26,240
O sea, hoy en día hasta Windows viene con un Python, digamos,

48
00:04:26,570 --> 00:04:30,940
se está no olvidando de los últimos 30 años en donde el Software Libre era mala palabra,

49
00:04:31,100 --> 00:04:35,520
y mismo Python viene, mismo Windows viene con Python y el sistema lo necesita.

50
00:04:35,720 --> 00:04:40,560
Con lo cual, craso error, ahí la decisión es prácticamente 99 a 1,

51
00:04:41,060 --> 00:04:42,520
correr en un entorno virtual.

52
00:04:43,460 --> 00:04:47,080
Y el último renglón, una vez que tenemos decidido que lo vamos

53
00:04:47,080 --> 00:04:49,840
a correr local y en un entorno de Python virtual,

54
00:04:50,560 --> 00:04:53,940
si vamos a usar una distribución de Python,

55
00:04:54,920 --> 00:04:58,380
la oficial de Python.org o una distribución propietaria.

56
00:04:59,020 --> 00:05:03,640
En nuestro caso, la decisión mía es correr una distribución

57
00:05:03,740 --> 00:05:04,300
propietaria.

58
00:05:05,780 --> 00:05:07,040
Y ahora vamos a ir a los detalles.

59
00:05:07,060 --> 00:05:09,420
Pero muy rápido ustedes, en todo caso, me frenan.

60
00:05:10,460 --> 00:05:15,820
si algo les llama la atención o si después nos queda tiempo por el tema de la idea es

61
00:05:15,820 --> 00:05:24,800
no robar tiempo de la clase del doctor Holik, digamos, me paran y me consultan.

62
00:05:25,380 --> 00:05:29,580
Bueno, de eso de arbolito de decisión que yo les digo, eran cuatro renglones, 16 opciones,

63
00:05:29,800 --> 00:05:36,339
acá vamos al segundo renglón, ¿qué pros y qué contras tenemos? Si decimos "che...

64
00:05:36,340 --> 00:05:37,780
Pero yo les quiero correr en la nube"

65
00:05:38,479 --> 00:05:42,760
Bueno, hay un tema con el correr en la nube, digamos,

66
00:05:42,990 --> 00:05:48,100
que es que una opción es Google Colab

67
00:05:50,840 --> 00:05:54,320
Que básicamente es una especie de entorno,

68
00:05:54,440 --> 00:05:56,360
como el que vamos a tener nosotros corriendo en nuestra

69
00:05:56,420 --> 00:05:57,000
mat, ¿qué que nada?

70
00:05:57,120 --> 00:05:59,640
Pero disfrazado de servicio en la nube,

71
00:05:59,760 --> 00:06:02,580
tiene una especie de front end.

72
00:06:03,200 --> 00:06:05,100
Pero en el back end es más o menos lo que estamos,

73
00:06:05,340 --> 00:06:06,320
lo que vamos a hacer nosotros.

74
00:06:06,620 --> 00:06:10,840
Y eso, en principio, uno diría "a mí que me importa" pero en la

75
00:06:10,860 --> 00:06:12,180
práctica trae problemas.

76
00:06:12,560 --> 00:06:17,060
La colaboración en el Google Colab es muy engorrosa.

77
00:06:17,140 --> 00:06:19,740
No es lo mismo trabajar--

78
00:06:19,980 --> 00:06:23,400
Por ejemplo, uno dice, "sí, pero yo trabajo con los Google

79
00:06:23,660 --> 00:06:25,440
Docs" y son buenísimos.

80
00:06:25,580 --> 00:06:28,940
Es el mejor paquete de oficina en la nube.

81
00:06:29,080 --> 00:06:30,140
Es el mejor lejos.

82
00:06:30,820 --> 00:06:31,640
Pero no es lo mismo.

83
00:06:31,860 --> 00:06:41,240
Google Colab no tiene la ferretería en el frontend que tiene el Google Docs. Y además,

84
00:06:41,400 --> 00:06:47,700
hay otro tema que es que uno ya vamos a ir en detalle, pero hay veces que le queda chico

85
00:06:47,860 --> 00:06:51,680
la potencia del procesamiento que te da el Google Colab y ahí tenés que pagar aparte,

86
00:06:51,780 --> 00:06:57,419
con lo cual es una cosa que podría tener problemas siempre, es bueno tener un entorno

87
00:06:57,420 --> 00:06:59,000
local como opción.

88
00:07:01,140 --> 00:07:04,160
Y una ventaja del entorno local muy grande de la ventaja que

89
00:07:04,160 --> 00:07:07,540
ustedes tienen control de la ferretería, digamos,

90
00:07:07,720 --> 00:07:11,400
a nivel de qué intérprete tienen,

91
00:07:11,480 --> 00:07:14,320
qué bibliotecas tienen instaladas, etcétera.

92
00:07:16,280 --> 00:07:18,940
Eso parecería una pedantería.

93
00:07:19,000 --> 00:07:20,840
Es decir, a mí me interesa ver la versión.

94
00:07:20,840 --> 00:07:21,240
No sé qué.

95
00:07:22,700 --> 00:07:26,619
Realmente el problema de trabajar con Google Colab es que

96
00:07:26,620 --> 00:07:30,380
cada vez que ustedes inician la sesión, vuelve a instalar,

97
00:07:30,620 --> 00:07:32,480
vuelve a hacer lo que vamos a hacer ahora nosotros a mano,

98
00:07:33,300 --> 00:07:35,520
lo base automáticamente cada vez que ustedes arrancan una

99
00:07:35,580 --> 00:07:36,480
sesión en Google Colab.

100
00:07:37,100 --> 00:07:39,520
Me pasó muchas veces que el entorno se pone demasiado

101
00:07:39,720 --> 00:07:42,640
pesado y capaz que está, no sé, 10 minutos instalando el

102
00:07:42,680 --> 00:07:43,900
entorno y termina fallando.

103
00:07:44,240 --> 00:07:47,760
Entonces, no es infalible el Google Colab.

104
00:07:48,940 --> 00:07:51,500
Cuando hablo de entorno en la nube--

105
00:07:51,520 --> 00:07:51,940
Perdón, Leandro

106
00:07:52,500 --> 00:07:52,580
Sí.

107
00:07:52,880 --> 00:07:53,140
Leandro, Hago una aclaración

108
00:07:53,400 --> 00:07:55,100
 que, por ahí es importante.

109
00:07:55,460 --> 00:07:58,800
tú estás poniendo en la nube, como ejemplo Google Colab,

110
00:07:59,380 --> 00:08:00,200
pero hay otras nubes, ¿no?

111
00:08:00,360 --> 00:08:02,420
Por ejemplo, yo corro en la--

112
00:08:02,440 --> 00:08:05,860
Por ejemplo, estos se les digo, los que se vayan a dedicar

113
00:08:05,860 --> 00:08:08,160
a investigación o que vayan a trabajar en una empresa,

114
00:08:09,600 --> 00:08:12,580
muy probablemente les hagan a usar AWS o Azure.

115
00:08:12,840 --> 00:08:15,300
Entonces ahí también van a tener que ir a la nube,

116
00:08:15,460 --> 00:08:17,180
sí o sí, por la potencia de cómputo.

117
00:08:17,500 --> 00:08:20,860
Si ustedes en su laptop van a acodear ligero,

118
00:08:20,960 --> 00:08:24,019
van a tener un editor de texto, o pueden hacerlo directamente

119
00:08:24,020 --> 00:08:25,180
en la tablet, ¿qué sé yo?

120
00:08:25,300 --> 00:08:26,740
Porque no van a estar corriendo a nada.

121
00:08:27,150 --> 00:08:30,120
Y cuando corren la cosa, no lo corren localmente porque no les

122
00:08:30,160 --> 00:08:31,300
da la potencia de computos.

123
00:08:31,310 --> 00:08:33,180
Entonces, lo mandan a un servidor.

124
00:08:33,530 --> 00:08:36,380
Y ahí sí o sí van a tener que interactuar con un servidor

125
00:08:36,419 --> 00:08:38,080
que típicamente no va a ser Colab,

126
00:08:38,360 --> 00:08:40,620
sino va a ser un servicio muchísimo mejor.

127
00:08:41,200 --> 00:08:43,479
Yo, por ejemplo, acá tengo acceso ahí a una súper

128
00:08:43,580 --> 00:08:44,920
computadora que está en Munich

129
00:08:45,440 --> 00:08:48,000
Que bueno, cuando tenemos que hacer una cuenta pesada,

130
00:08:48,090 --> 00:08:48,760
lo mandamos ahí.

131
00:08:48,810 --> 00:08:50,540
Y ahí también aparece una Jupyter Notebook

132
00:08:51,340 --> 00:08:54,060
yo puedo controlar qué paquetes de instal o qué no instal,

133
00:08:54,080 --> 00:08:55,780
o me puedo hacer un entorno de Python ahí.

134
00:08:56,620 --> 00:08:57,720
Como si fuera mi computadora.

135
00:08:58,080 --> 00:09:01,140
Entonces, ¿lo del local global?

136
00:09:01,360 --> 00:09:03,780
Bueno, a veces conviene global, a veces conviene local.

137
00:09:04,239 --> 00:09:05,300
Típicamente conviene global.

138
00:09:05,500 --> 00:09:07,920
Se van a hacer tareas de supercomputo,

139
00:09:07,960 --> 00:09:10,500
todo lo que demande mucho computo,

140
00:09:10,560 --> 00:09:14,840
o conviene hacerlo en la nube, porque no les va a dar el cuero

141
00:09:14,880 --> 00:09:16,860
para hacerlo en su computadora personal.

142
00:09:17,240 --> 00:09:18,700
Es una aclación importante.

143
00:09:19,900 --> 00:09:21,300
Sí, de acuerdo, de acuerdo.

144
00:09:22,820 --> 00:09:23,840
Entiendo que está--

145
00:09:23,960 --> 00:09:26,320
Mis 10 minutos acá van a ser un poco tendenciosos,

146
00:09:26,460 --> 00:09:27,380
porque yo estoy promoviendo.

147
00:09:27,400 --> 00:09:28,020
- Ya era pasará.

148
00:09:28,030 --> 00:09:28,420
- Como local.

149
00:09:29,240 --> 00:09:30,800
Pero estaba justamente por decir eso.

150
00:09:30,880 --> 00:09:34,940
De hecho, de hecho, a ver.

151
00:09:36,720 --> 00:09:40,740
Miren, esto que vamos a instalar localmente en unos

152
00:09:40,960 --> 00:09:46,020
minutitos, por ejemplo, esta es la versión, digamos, pura,

153
00:09:46,560 --> 00:09:48,980
pura, pero corriendo en la nube, o sea,

154
00:09:49,060 --> 00:09:54,900
software libre puro pero corriendo en la nube, que justamente también es una posibilidad.

155
00:09:55,540 --> 00:10:00,860
Los cuadernos Jupyter, bueno eso es lo que decía el Dr. Holik, pero vuelvo a la

156
00:10:00,900 --> 00:10:18,500
presentación así, así este... ahi esta, vuelva la presentación. Bueno entonces una vez que decidimos

157
00:10:18,820 --> 00:10:22,920
en todo caso correr con el entorno local tenemos que decidir si vamos a usar el entorno de sistema

158
00:10:23,220 --> 00:10:29,979
o un entorno Python virtual, claramente es un error usar el entorno de sistema, vamos a crear

159
00:10:29,980 --> 00:10:32,560
un entorno virtual del sistema operativo.

160
00:10:32,720 --> 00:10:34,100
Vamos a correr un entorno virtual.

161
00:10:35,000 --> 00:10:36,720
El tema compaitones que, como ustedes saben,

162
00:10:36,880 --> 00:10:38,100
es un lenguaje interpretado.

163
00:10:38,300 --> 00:10:40,100
Tiene un intérprete que pasa a Bicode,

164
00:10:40,260 --> 00:10:43,600
si le va a ir a Bicode, digamos, a código máquina.

165
00:10:44,240 --> 00:10:47,180
Pero además de eso, es una distribución que tiene un

166
00:10:47,540 --> 00:10:49,660
montón de bibliotecas, en este caso,

167
00:10:49,920 --> 00:10:52,680
lo que se llama con mayúsculas bibliotecas estándar.

168
00:10:54,079 --> 00:10:56,280
Y no solo la biblioteca estándar,

169
00:10:56,280 --> 00:10:58,040
por supuesto, va a estar en cualquier instalación.

170
00:10:58,140 --> 00:10:59,880
Pero una vez que hacemos un entorno virtual,

171
00:11:00,070 --> 00:11:05,520
ese entorno virtual incluye bibliotecas que nosotros vamos

172
00:11:05,720 --> 00:11:07,620
a instalar a mano.

173
00:11:07,980 --> 00:11:12,720
Entonces, es otra ventaja de usar un entorno virtual.

174
00:11:12,960 --> 00:11:17,320
Ahora, como parte de las bibliotecas que vamos a instalar

175
00:11:17,510 --> 00:11:21,899
a mano, digamos, está el tema de un servidor de cuaderno

176
00:11:21,900 --> 00:11:27,100
local. Dos palabras de qué es un cuaderno de su

177
00:11:27,120 --> 00:11:33,040
píter. Lo que estábamos viendo recién, ustedes pueden correr localmente, esto que

178
00:11:33,040 --> 00:11:42,080
se ve en la nube, que es cuadernos, cuadernos, voy a ver un ejemplo cualquiera,

179
00:11:43,760 --> 00:11:51,880
cuadernos en donde tienen células de texto, markdown, markdown y markdown, realmente hay

180
00:11:51,880 --> 00:12:01,160
enchamigarse con Markdown porque es los próximos 200 años de la

181
00:12:01,430 --> 00:12:08,880
de "computación de usuario final". Pero además, las celdas que son celdas de Markdown de texto

182
00:12:09,520 --> 00:12:16,940
pueden poner celdas programables que el servidor Jupiter va a ejecutar y les va a dar un resultado.

183
00:12:20,140 --> 00:12:26,560
Si, si tiene razón Marcos, es re-amigable Markdown, básicamente es un HTML recontra

184
00:12:26,600 --> 00:12:33,760
destilado para poder tipearse digamos de corrido sin necesitar las etiquetas de HTML,

185
00:12:33,860 --> 00:12:38,520
así que, pero incluso se puede incrustar HTML en Markdown, eso lo hago acá en la presentación

186
00:12:39,080 --> 00:12:39,640
más de una vez.

187
00:12:40,620 --> 00:12:46,279
Fíjense que esta presentación está hecha en Markdown y ven que acá le metí etiquetas

188
00:12:47,780 --> 00:12:55,500
de su índice, digamos, que es html, pero no importa, no me voy a desviar, sigo con que

189
00:12:55,500 --> 00:13:04,080
es un cuaderno Jupyter, entonces son celdas en donde tienen celdas ejecutables y el cuaderno

190
00:13:04,100 --> 00:13:11,279
Jupyter por más que tiene una extensión propietaria, digamos, es un JSON, es un JSON, es un archivo

191
00:13:11,280 --> 00:13:20,040
texto, "Jota-SON" con lo cual se puede sincronizar via Git sin ningún problema, pero una cosa

192
00:13:20,040 --> 00:13:26,620
que es muy piola que no solo sincroniza las celdas de texto y las celdas ejecutables sino

193
00:13:26,620 --> 00:13:33,360
que además serializa y guarda en el que ya son los resultados, entonces uno puede ver un cuaderno

194
00:13:33,380 --> 00:13:40,520
Jupyter sin volver a ejecutarlo y tiene los mismos resultados que tuvo la autora original.

195
00:13:40,600 --> 00:13:45,600
Entonces eso es un cuaderno de Jupyter, no voy a ir más en detalle, pero quiero mostrar

196
00:13:45,720 --> 00:13:50,400
una cosa que tiene que ver con lo que decía recién el doctor Holik, que es esto.

197
00:13:51,260 --> 00:13:54,580
Esta es un poquito mínimo-mínimo la arquitectura de un servidor Jupyter.

198
00:13:55,020 --> 00:14:04,079
Tenemos un navegador que va a dar ser la GUI, que se conecta a un servidor que en nuestro caso

199
00:14:04,080 --> 00:14:10,140
correría local en su máquina y este servidor a su vez va a estar conectado

200
00:14:10,640 --> 00:14:19,520
vía un protocolo de mensajes, un MQ (colas de mensajes) a un kernel, un núcleo

201
00:14:19,550 --> 00:14:24,620
que ese kernel se ejecuta a las celdas ejecutables. Una cosa muy importante es

202
00:14:24,620 --> 00:14:28,100
que el kernel podría ser Python pero también puede ser cuando lo corremos

203
00:14:28,200 --> 00:14:33,340
local, tenemos muchas opciones, puede ser SQLite, puede ser C,

204
00:14:33,360 --> 00:14:43,700
puede ser Julia, puede ser R (para quien se anime). Y además este servidor va a grabar este

205
00:14:43,740 --> 00:14:49,180
archivo JSON en forma local en su computadora, entonces después ustedes lo pueden sincronizar,

206
00:14:49,380 --> 00:14:54,560
por ejemplo, vía Git a GitHub, por ejemplo, o cualquier servidor Git que ustedes les interese.

207
00:14:54,560 --> 00:15:00,479
O sea, esto les da muchísimas opciones, fíjense que abrí cuatro bloquecitos y tenemos muchísimas

208
00:15:00,480 --> 00:15:08,020
opciones, pero son opciones que no molestan porque básicamente todo el tiempo lo que van a hacer

209
00:15:08,140 --> 00:15:13,940
es archivo guardado local, se han realizado por Git y se acabó, es un proceso es un proceso muy

210
00:15:15,540 --> 00:15:23,580
muy simple. Bueno, para no extenderme mucho acá les dejo comparaciones de distribución

211
00:15:23,740 --> 00:15:29,719
propietaria a ver sus distribución estándar, vamos a usar la distribución propietaria en este

212
00:15:29,720 --> 00:15:35,020
pues en este caso es Anaconda. ¿Cómo instalamos Anaconda? De nuevo, Anaconda es una empresa,

213
00:15:35,600 --> 00:15:43,040
una "Inc", una punto com, que se dedica a hacer lo mismo que Python.org, pero es decir,

214
00:15:43,340 --> 00:15:50,920
hace una distribución de Python, pero se dedica a tener una biblioteca, mejor hecho un repositorio

215
00:15:50,920 --> 00:16:01,560
de bibliotecas, de libraries que están, digamos, eso muy prolijas, sobre todo para, sobre todo

216
00:16:01,620 --> 00:16:08,560
para lo que es temas de ciencia de datos, temas de ciencia de datos y cosas de dominio específico.

217
00:16:08,920 --> 00:16:14,780
Por ejemplo, si van a trabajar con GPUs y con NVIDIA, no queda otra que usar esta distribución,

218
00:16:15,260 --> 00:16:20,900
lamentablemente sufrí eso. Les dejo en la presentación el tutorial de instalación de

219
00:16:20,900 --> 00:16:28,500
en Windows, la verdad yo en Windows no lo puedo probar, no tengo Windows a mano, pero no debería

220
00:16:28,500 --> 00:16:35,300
dar ningún problema, digamos, si en Linux, si en MacOS anda, Windows debería ser todavía más directo.

221
00:16:36,200 --> 00:16:44,780
Es directo en los nuevos? En Windows se descargan el instalador, le cliquen y le ejecutan y se hace

222
00:16:44,780 --> 00:16:50,340
solo y después lo lanzan y después bueno después les enseñe usarlo. Meo que Windows

223
00:16:50,410 --> 00:16:55,180
es trivial instalarlo y en Python más o menos también lo pueden saber, lo voy a explicar

224
00:16:55,260 --> 00:17:00,280
supongo ahora Leandro. Es trivial en cualquiera de los sistemas de operativos, de eso vive

225
00:17:00,440 --> 00:17:05,480
Anaconda, de eso vive y realmente prospera: de hacer lo mismo que Python 

226
00:17:05,500 --> 00:17:14,380
pero un poquito más, digamos, amigable. más que amigable y que realmente sea muy multiplataforma,

227
00:17:14,459 --> 00:17:17,760
Fíjense que acá en este tutorial les hice. 

228
00:17:19,560 --> 00:17:20,260
Dos minutos más.

229
00:17:20,579 --> 00:17:21,459
Sí, dos minutos más.

230
00:17:22,459 --> 00:17:23,880
Fíjense que acá les dice, bueno,

231
00:17:24,020 --> 00:17:25,380
cómo probar el entorno, etcétera.

232
00:17:25,439 --> 00:17:27,060
Vamos a hacer--

233
00:17:27,180 --> 00:17:28,580
Miren, yo ya lo tengo instalado acá.

234
00:17:28,820 --> 00:17:36,320
Lo que voy a hacer es mostrarles en mi máquina cómo es crear un

235
00:17:44,000 --> 00:17:44,440
entorno--

236
00:17:54,880 --> 00:18:03,060
Este archivo que está acá dice c25.yaml, si lo vemos, eso también está compartido

237
00:18:03,060 --> 00:18:08,880
en la presentación, si lo vemos es un archivo bueno, yaml de texto que le dice en este caso

238
00:18:09,060 --> 00:18:16,640
a Conda que es el ejecutable que viene con Anaconda le dice cómo crear un nuevo entorno,

239
00:18:16,860 --> 00:18:24,940
¿sí? Es equivalente al requirements.txt que viene en la distribución estándar. Pero

240
00:18:24,940 --> 00:18:39,040
no es un txt, es un yaml, ya tiene una ventaja importante. Obviamente, 511404. Bueno, este

241
00:18:39,040 --> 00:18:49,240
este es el entorno que vamos a crear hoy y estamos creando un entorno nuevo, por supuesto,

242
00:18:51,220 --> 00:18:59,920
de nuevo, con más razón Linux viene con la distribución Python Standard que hay que

243
00:18:59,920 --> 00:19:07,420
evitar usar, no por ser standards sino porque es la que usa el sistema operativo.

244
00:19:09,260 --> 00:19:26,340
Me mande una macana, eso de 25.11.04, 25.11.04, ¿por qué no encuentra el? No encuentra

245
00:19:26,340 --> 00:19:32,520
la anaconda. Bueno, todas las demos tienen que fallar si no nos hondemos.

246
00:19:40,620 --> 00:19:45,300
Bueno, hay una forma por ahí fácil o visual de armarlo al entorno que es con el...

247
00:19:46,220 --> 00:19:50,140
Cuando está la anaconda hay un navegador de anaconda. Entonces cuando abre el

248
00:19:50,320 --> 00:19:54,800
navigator hay una forma absolutamente con ventanitas de crear un entorno.

249
00:19:54,980 --> 00:20:02,860
Yo después les enseño esa que es por ahí un poco más fácil que la de la terminal de comando.

250
00:20:03,260 --> 00:20:06,500
Esa también la pueden usar, los que quieren, puedes hacer la guía.

251
00:20:07,179 --> 00:20:10,580
Perfecto, perfecto. Sí, pero no sé por qué no me encuentra...

252
00:20:13,720 --> 00:20:18,060
Bueno, lo pasé a mi cambio de máquina y lo probé en la otra típico de demo.

253
00:20:19,420 --> 00:20:22,240
Tengo instalado acá el Anaconda, no sé.

254
00:20:22,980 --> 00:20:23,860
Bueno, no importa.

255
00:20:24,440 --> 00:20:29,980
Creame, entonces, que cuando tienen instalado Anaconda con este comando,

256
00:20:30,910 --> 00:20:34,660
les crea un entorno nuevo.

257
00:20:37,340 --> 00:20:39,740
Marcos, acá, apoya la moción.

258
00:20:40,130 --> 00:20:45,700
De todas maneras, de nuevo, el crear un entorno también está en la demo que les dejo.

259
00:20:48,070 --> 00:20:48,740
Una vez que está.

260
00:20:49,460 --> 00:20:53,220
pero yo estoy seguro que acá lo tengo instalado en Anaconda.

261
00:20:53,460 --> 00:20:54,920
Bueno, debe ser que no lo tengo instalado.

262
00:20:55,400 --> 00:20:56,460
La cuestión es que--

263
00:21:02,860 --> 00:21:04,160
La cuestión es que--

264
00:21:05,770 --> 00:21:06,300
Miren, un segundo.

265
00:21:09,440 --> 00:21:13,960
La cuestión es que cuando ustedes tienen instalado y creado

266
00:21:14,020 --> 00:21:15,140
un entorno nuevo--

267
00:21:19,200 --> 00:21:30,440
Vamos. Lo activan con un comando de activación que también está acá en el tutorial que

268
00:21:30,440 --> 00:21:40,380
les dejó, que les dejé al principio cuando activan el entorno. Acá les aparece que le

269
00:21:40,480 --> 00:21:46,140
como estoy corriendo bajo un entorno, estoy corriendo bajo un entorno que por ejemplo les permite correr

270
00:21:49,019 --> 00:21:52,200
ciertos comandos,

271
00:21:57,820 --> 00:22:03,080
que si no lo tienen activado (como ahora) cuando tratan de correr el comando no lo pueden correr,

272
00:22:04,080 --> 00:22:11,020
dice que el comando no existe. Entonces el entorno, digamos, justamente cuando ustedes

273
00:22:11,160 --> 00:22:20,600
instalan un comando, cuando ustedes instalan, como dijimos antes, un entorno nuevo y como

274
00:22:20,700 --> 00:22:32,440
dijimos antes, este es el archivo que describe el entorno, les deja dentro del entorno, las

275
00:22:32,440 --> 00:22:40,480
como se llaman las, los comandos a disposición. Por ejemplo este, este archivo que les estoy

276
00:22:40,540 --> 00:22:48,440
mostrando ya les instale el Jupyter-Lab para correr localmente lo mismo que tendrían en el,

277
00:22:51,160 --> 00:23:02,420
como se llama.... en la nube. Sí, bueno, creo que por una cuestión de tiempo, creo que por una

278
00:23:02,420 --> 00:23:10,540
de tiempo lo vamos a dejar acá. Vamos a la sección de preguntas si les parece. Acá les muestro

279
00:23:10,680 --> 00:23:18,200
cómo una vez que activan el entorno virtual, corren este comando de su paiter lado y ejecuta

280
00:23:20,640 --> 00:23:26,360
el servidor que como habíamos dicho antes, un segundo que tenía por acá.

281
00:23:31,180 --> 00:23:36,600
Bueno, de nuevo, les cambia el prompt, como habíamos dicho antes, y les muestra el 

282
00:23:36,780 --> 00:23:37,020
Jupyter-Lab

283
00:23:38,720 --> 00:23:39,240
Conclusiones.

284
00:23:40,680 --> 00:23:46,520
Tienen las opciones de correrlo local o correrlo remoto. Dentro de local: una distribución propietaria

285
00:23:46,580 --> 00:23:48,020
que es Anaconda, que es la recomendada.

286
00:23:49,130 --> 00:23:55,620
De hecho, el entorno que se están llevando también incluye la instalación de Qiskit

287
00:23:56,200 --> 00:23:57,620
para poder hacer las simulaciones.

288
00:23:57,940 --> 00:24:00,060
Y realmente, cuando les instale el entorno,

289
00:24:00,440 --> 00:24:03,480
ya les deja el Qiskit instalado para hacer las

290
00:24:03,580 --> 00:24:04,060
simulaciones.

291
00:24:07,220 --> 00:24:07,520
Bien.

292
00:24:07,880 --> 00:24:09,800
Bueno, se me fue el tiempo.

293
00:24:10,080 --> 00:24:12,160
¿Alguna pregunta?

294
00:24:12,560 --> 00:24:12,780
Estoy.

295
00:24:15,100 --> 00:24:19,880
Leandro, estaría bueno que lo compartas a esto por el

296
00:24:19,960 --> 00:24:22,520
chat y que lo mandes al grupo de WhatsApp,

297
00:24:23,820 --> 00:24:26,120
a la comunidad de WhatsApp, así le queda a todo el mundo,

298
00:24:26,180 --> 00:24:27,180
incluso a los que no vinieron.

299
00:24:27,900 --> 00:24:29,440
Sí, sí, sí, sí, perfecto.

300
00:24:29,580 --> 00:24:31,420
Todo al compartir el enlace al principio,

301
00:24:31,720 --> 00:24:32,820
ya lo comparto por el chat.

302
00:24:34,800 --> 00:24:37,580
Si no hay más preguntas entonces, dejo de compartir.

303
00:24:47,940 --> 00:24:54,300
Me cambie de compu y se complica un poco con la--

304
00:24:54,300 --> 00:24:54,820
A lo que va a hacer.

305
00:24:55,040 --> 00:24:55,240
¿Listo?

306
00:24:58,280 --> 00:25:05,060
Para probar siempre es un desafío, porque siempre hay kilombitos.

307
00:25:05,140 --> 00:25:08,100
Por eso les digo, ustedes, en sus casadas,

308
00:25:08,220 --> 00:25:11,920
en sus sistemas operativos y de la forma más fácil que encuentren,

309
00:25:12,000 --> 00:25:15,000
les queda como ejercicio instalarse anaconda,

310
00:25:15,880 --> 00:25:19,980
abrir un ejemplo de Jupyter Notebook y correr Python,

311
00:25:20,260 --> 00:25:23,080
alguna versión, la que sea, hacer "1+1"

312
00:25:23,180 --> 00:25:27,540
les tiene que dar "2", ¿ok? ¿Por qué iba a hacer esa tarea tan tonta? Bueno, porque

313
00:25:27,580 --> 00:25:32,880
muchas veces pasa lo que le pasó a Leandro recién: siempre pasa algo, sobre todo para

314
00:25:32,960 --> 00:25:38,100
los que están ahí con la terminal, con Linux. todos los linuxeros son iguales,

315
00:25:38,180 --> 00:25:42,460
¿viste? Te dicen "no, no, pero es refácil, no, pero mira, es refácil, no volvés".

316
00:25:42,460 --> 00:25:47,460
Y empieza, "no, para lo que me falta, me falta instalar esta guiasita tres horas, ¿viste

317
00:25:48,280 --> 00:25:52,800
siempre pasa lo mismo. Bueno, ¿por qué es importante que lo van como ejercicio?

318
00:25:54,480 --> 00:25:58,620
Si te pasa, no pasa eso, es que no sabes qué estás instalando básicamente.

319
00:25:59,760 --> 00:26:05,920
Es que no, exacto, es que la mayoría, mira, el 90% de los usuarios no sabe lo que está instalando.

320
00:26:06,020 --> 00:26:17,440
Esa es la realidad del mundo. Entonces, la pregunta es, ¿cómo poder hacer algo en ese

321
00:26:17,440 --> 00:26:21,160
un usuario avanzado va a tener la computadora siempre a punto que se yo,

322
00:26:21,320 --> 00:26:27,320
eso va a pasar. Pero qué hacer con el resto de los usuarios? Lo que es

323
00:26:27,360 --> 00:26:30,680
muy importante es que ustedes como ejercicio hagan esto en sus casas, que se

324
00:26:30,740 --> 00:26:37,620
instalen anaconda, que abran un Jupyter Notebook de la manera que sea y que la

325
00:26:37,680 --> 00:26:42,380
corran, que les corra Python. Obviamente a la mayoría no le va a salir,

326
00:26:42,740 --> 00:26:46,720
la vez que viene seguimos, porque ya la vez que viene les voy a poner

327
00:26:46,720 --> 00:26:56,800
directamente los ejes. Exacto, exacto, siente, siente. La vez que viene ya los ejemplos del curso

328
00:26:56,900 --> 00:27:03,880
van a ser con Python, ok? Yo voy a abrir una un editor de Python y vamos a correr cosas ahí,

329
00:27:04,030 --> 00:27:11,820
ok? Pero hoy sigo y agradecemos a Leandro por esta explicación. Sí, Leandro. Dos aclaraciones,

330
00:27:12,020 --> 00:27:16,700
confirmó que no tenía Anaconda instalado en esta máquina. o sea, yo practiqué la demo en la compu de mi casa, 

331
00:27:16,700 --> 00:27:21,960
ahora estoy en la oficina no tengo en esta máquina Anaconda instalado con lo cual digamos

332
00:27:22,140 --> 00:27:27,940
"nunca falla la teoría, lo que fallan son las hipótesis"... usted lo debe saber doctor y la otra cosa es que

333
00:27:28,230 --> 00:27:36,100
me tengo que retirar a otra clase en otro lado. Así que por eso estoy huyendo no por el papelón

334
00:27:36,170 --> 00:27:42,019
sino porque realmente me tengo que retirar. 
-Gracias a la muchas gracias por el tutorial y

335
00:27:42,020 --> 00:27:44,760
y queda compartido, así que ya lo tienen, pero eso.

336
00:27:46,060 --> 00:27:48,020
Yo después sigo, la vez que viene,

337
00:27:48,100 --> 00:27:49,100
lo seguimos viendo de nuevo.

338
00:27:49,660 --> 00:27:53,020
No se preocupen, pero nada, les queda de ejercicio

339
00:27:53,640 --> 00:27:54,600
instalarse Python.

340
00:27:55,760 --> 00:27:59,620
Bien, entonces, ahora paso a compartir pantalla yo.

341
00:28:05,060 --> 00:28:09,340
Y vamos a seguir viendo cosas de espacios vectoriales.

342
00:28:10,260 --> 00:28:14,460
Y ya hoy vamos a empezar a ver con portas lógicas cuánticas y circuitos cuánticos.

343
00:28:14,780 --> 00:28:18,720
Y vamos a tratar de explicar un poco la noción de entelazamiento cuántico.

344
00:28:19,540 --> 00:28:21,440
A este era así.

345
00:28:23,120 --> 00:28:24,080
Bien, perfecto.

346
00:28:25,680 --> 00:28:31,140
Faltaron ver algunas cositas de propiedades de los sistemas cuánticos.

347
00:28:31,220 --> 00:28:33,340
Vamos a ver ahora observables y valores medios.

348
00:28:34,840 --> 00:28:37,120
¿Qué significa un observable cuántico?

349
00:28:37,560 --> 00:28:39,020
Y cómo se calcula un valor medio.

350
00:28:39,180 --> 00:28:45,480
Bien, por lo que veníamos viendo hasta ahora, el estado de un sistema cuántico viene dado por un vector,

351
00:28:46,380 --> 00:28:48,340
un vector en un espacio vectorial, ¿sí?

352
00:28:49,440 --> 00:28:51,900
Y el símbolo era el "psi", ¿no?

353
00:28:52,860 --> 00:28:55,340
A esto, de ahora en más, lo vamos a llamar "ket".

354
00:28:56,080 --> 00:28:56,900
Ahora van a ver por qué.

355
00:29:00,540 --> 00:29:06,220
El observable que representaría a lo que estamos estudiando físicamente, por ejemplo, a la vez pasada,

356
00:29:06,520 --> 00:29:11,340
Habíamos visto la propiedad de spin, que era una propiedad de que si poníamos un campo magnético,

357
00:29:11,940 --> 00:29:15,780
el rayo de partículas se podría defectar para arriba o para abajo,

358
00:29:16,020 --> 00:29:20,820
en alguna de las dos direcciones que quedan definidas por el campo magnético,

359
00:29:22,260 --> 00:29:27,380
o podría ser la energía, o podría ser el momento angular, o cualquier otra magnitud física

360
00:29:28,919 --> 00:29:31,880
que querramos estudiar acerca del sistema.

361
00:29:32,060 --> 00:29:33,700
A eso le vamos a llamar observable.

362
00:29:33,820 --> 00:29:35,640
Piensen para fijar ideas en la energía.

363
00:29:36,620 --> 00:29:44,400
o en la posición, o en lo que quieran, puede ser espin también, pero lo importante en cuántica es que el observable va a

364
00:29:44,400 --> 00:29:50,340
que ha representado por una matriz armítica, ¿sí? y una matriz armítica va a ser una matriz cuadrada

365
00:29:51,300 --> 00:29:58,080
con entradas complejas, es decir, una matriz de complejos n por n tal que a es igual a a

366
00:29:58,080 --> 00:30:06,880
transpuesta conjugada. Esto de acá, adaga, ven por qué, ahora estuve practicando esto,

367
00:30:09,000 --> 00:30:19,220
igual adaga significa, esto de adaga quiere decir por definición a transpuesta y conjugada.

368
00:30:23,100 --> 00:30:29,780
¿Qué quiere decir a transpuesta conjugada? Bueno, quiere decir que cambian chilas por columnas. Voy a borrar acá.

369
00:30:34,480 --> 00:30:36,580
Por ejemplo, vamos a la...

370
00:30:39,520 --> 00:30:44,620
Supongo que tiene una matriz así, ¿no? Que es eso, 0 menos i y 0.

371
00:30:45,780 --> 00:30:47,220
Vamos a hacer a transpuesta.

372
00:30:48,300 --> 00:30:51,640
Tengo que intercambiar chilas por columnas. Entonces, esta chila

373
00:30:52,480 --> 00:30:53,940
pasa a ser una columna.

374
00:30:54,780 --> 00:30:57,000
Esta columna pasa a ser una fila.

375
00:31:01,179 --> 00:31:03,960
Y esa columna pasa a ser una fila.

376
00:31:05,560 --> 00:31:07,040
Entonces, esta es atraspuesta.

377
00:31:10,180 --> 00:31:11,280
Y cuando conjugó,

378
00:31:13,800 --> 00:31:14,840
ahora tengo que conjugar,

379
00:31:15,380 --> 00:31:17,620
este chibinbolito significa conjugar.

380
00:31:17,620 --> 00:31:20,340
Tengo que conjugar cada una de las entradas de la matriz.

381
00:31:20,640 --> 00:31:26,200
con jugo de cero y con jugo de -i, -i con jugo de i y cero con jugo de cero.

382
00:31:26,860 --> 00:31:30,280
Entonces fíjense que en este caso ha transpuesto a con jugo de a que es por

383
00:31:30,320 --> 00:31:37,520
definición a daga diodivalado. Entonces los observables, las magnitudes

384
00:31:37,680 --> 00:31:41,880
físicas, en física cuántica se representan matemáticamente por matrices

385
00:31:41,940 --> 00:31:46,560
que cumplen que a daga esivala a y estas son matrices permíticas.

386
00:31:50,860 --> 00:31:55,000
Bien, seguimos con la presentación.

387
00:31:58,310 --> 00:32:13,460
Esto no lo dije hasta ahora, pero le voy a decir ahora que los valores posibles que puede tomar un observable, una magnitud física a medir, van a ser y solamente pueden ser los autóvalores de la matriz que representa dicho observable.

388
00:32:13,840 --> 00:32:17,200
Ahora voy a explicar lo que es un autovalor y lo que es un autovector, ¿sí?

389
00:32:17,700 --> 00:32:20,440
Pero la idea es esa que, dado el observable,

390
00:32:23,280 --> 00:32:24,720
que sería una magnitud física,

391
00:32:26,040 --> 00:32:27,640
por ejemplo, la energía,

392
00:32:29,730 --> 00:32:30,540
la energía,

393
00:32:32,980 --> 00:32:35,700
la energía va a estar representada por una matriz

394
00:32:36,980 --> 00:32:38,080
y los posibles valores

395
00:32:39,320 --> 00:32:41,580
van a ser los que pueda tomar la energía,

396
00:32:42,480 --> 00:32:44,000
van a ser los autovalores.

397
00:32:44,580 --> 00:32:47,940
Y los autovalores son unos números reales,

398
00:32:48,380 --> 00:32:51,340
números complejos, no, si, números reales que cumplen

399
00:32:52,140 --> 00:32:55,080
con la ecuación de autovalores y autovectores.

400
00:32:55,200 --> 00:32:58,720
Y eso lo voy a explicar ahora, acto seguido, después de estar de positiva.

401
00:32:59,900 --> 00:33:01,460
Entonces, esa va a ser la idea, ¿no?

402
00:33:03,480 --> 00:33:08,840
Bien, entonces, los valores posibles que pueda tomar la magnitud

403
00:33:08,980 --> 00:33:11,960
cuando hacen un experimento van a ser los autovalores de la matriz.

404
00:33:12,340 --> 00:33:14,740
y les decía, y esto sí lo vimos la vez pasada,

405
00:33:14,800 --> 00:33:18,420
es que la evolución dinámica va a estar dada por una matriz unitaria.

406
00:33:18,500 --> 00:33:26,280
Entonces, el estado del sistema cuántico en el tiempo t va a venir dada por la multiplicación

407
00:33:26,800 --> 00:33:33,600
entre la matriz unitaria que representa la evolución u por el vector de estado en el tiempo inicial.

408
00:33:34,700 --> 00:33:38,380
Entonces, las comportas lógicas cuánticas van a ser estas u de acá,

409
00:33:39,080 --> 00:33:42,100
van a ser instancias de evoluciones unitarias.

410
00:33:43,040 --> 00:33:46,360
Hoy vamos a ver ejemplos de comportas lógicas cuánticas.

411
00:33:46,680 --> 00:33:49,120
Estas "u" son las comportas lógicas.

412
00:33:52,060 --> 00:33:53,340
¿Y qué hacen las comportas lógicas?

413
00:33:53,420 --> 00:33:57,060
Bueno, transforman el estado de la memoria de la computadora cuántica.

414
00:33:57,420 --> 00:34:00,560
Uno inicia a la computadora en el estado obsiciero,

415
00:34:01,080 --> 00:34:02,640
esto es a "t" igual a 0,

416
00:34:03,680 --> 00:34:05,940
y después de que uno le aplique una comporta lógica,

417
00:34:06,120 --> 00:34:12,240
ahora el estado de la computadora cuántica cambia y se vuelve t.

418
00:34:12,440 --> 00:34:12,560
¿Sí?

419
00:34:15,640 --> 00:34:16,040
Bien.

420
00:34:18,460 --> 00:34:21,639
Y con los autovalores y autovactores que se les voy a explicar ahora,

421
00:34:21,919 --> 00:34:22,659
uno puede...

422
00:34:24,260 --> 00:34:26,960
Ah, esto, acá me falta... Perdón, me faltó...

423
00:34:29,200 --> 00:34:29,800
Me falta algo.

424
00:34:36,000 --> 00:34:37,520
Me faltó esto acá.

425
00:34:38,220 --> 00:34:44,260
Uno puede reescribir a la matriz que representa al observable de una manera muy especial, que es la descomposición espectral.

426
00:34:46,879 --> 00:34:54,280
La otra cosa que estuvimos viendo en el curso es el principio de superposición. Implicitamente, ahora se los digo formalmente,

427
00:34:54,770 --> 00:34:59,540
si uno tiene un sistema cuántico que puede estar en los estados Psi1 y Psi2,

428
00:35:00,100 --> 00:35:06,140
uno puede armar una combinación lineal de esos dos vectores y producir un nuevo estado,

429
00:35:06,700 --> 00:35:10,580
si, siempre y cuando, la norma de si sea igual a 1.

430
00:35:11,640 --> 00:35:16,600
Entonces, dados dos vectores de norma 1 que representan a estados cuánticos,

431
00:35:16,760 --> 00:35:19,640
uno puede, haciendo la combinación lineal,

432
00:35:21,060 --> 00:35:28,580
producir un nuevo estado cuántico, siempre y cuando la norma del vector generado sea 1.

433
00:35:29,960 --> 00:35:35,600
Fíjense que esto sería el gato de Schrodinger porque si uno tiene el gato por ejemplo gato vivo, ¿no?

434
00:35:40,070 --> 00:35:42,080
Y tiene el estado gato muerto, ¿no?

435
00:35:46,820 --> 00:35:51,040
Uno puede siempre generar una superposición por ejemplo hace la combinación lineal

436
00:35:52,240 --> 00:35:56,319
1 sobre raíz de 2 por gato vivo más 1 sobre raíz de gato

437
00:35:56,840 --> 00:36:04,220
2 por 4. Esto sería el alfa 1 por si 1, más el alfa 2 por si 2.

438
00:36:05,520 --> 00:36:10,120
Entonces la combinación lineal representa a los estados de superposición

439
00:36:10,960 --> 00:36:19,920
y esto sería lo que se conoce en la jerga como estados de superposición.

440
00:36:20,040 --> 00:36:23,040
Entonces cada vez que escuchen la noción de estado de superposición,

441
00:36:23,340 --> 00:36:27,600
piensa que estamos haciendo referencia a una combinación lineal de Estados.

442
00:36:28,520 --> 00:36:31,180
Y la otra cosa importante es que las matrices unitarias,

443
00:36:31,480 --> 00:36:34,120
es decir, aquellas que dan lugar a la evolución temporal,

444
00:36:35,060 --> 00:36:39,140
tienen que cumplir con esta ecuación de acá abajo.

445
00:36:40,020 --> 00:36:40,800
Que U...

446
00:36:44,820 --> 00:36:47,660
(Perdón, acá de vuelta, me equivoqué.)

447
00:36:47,720 --> 00:36:49,060
Tiene que ser U a la -1.

448
00:36:50,120 --> 00:36:52,380
(Perdón, no, no, no.)

449
00:36:52,380 --> 00:36:56,120
tiene que ser igual a "u", entonces "u" por "u"

450
00:37:01,000 --> 00:37:07,720
"u" por "u" tiene que ser igual a "u", y esto tiene que ser igual a la matriz identidad

451
00:37:08,780 --> 00:37:15,060
Esta es la convisión que tienen que cumplir las matrices que dan lugar a la evolución temporal

452
00:37:15,400 --> 00:37:20,920
Ahora, atención, es diferente de esta condición, no?

453
00:37:21,030 --> 00:37:22,280
Yo antes la había puesto mal.

454
00:37:22,420 --> 00:37:24,240
Esta es la condición de hermiticidad.

455
00:37:25,760 --> 00:37:26,440
Hermiticidad, sí.

456
00:37:27,180 --> 00:37:28,400
Esta es la hermiticidad.

457
00:37:29,060 --> 00:37:33,600
Y esta condición de acá es que la inversa de U

458
00:37:33,880 --> 00:37:35,540
tiene que ser su transpuesta conjugada.

459
00:37:36,380 --> 00:37:39,980
Entonces, los observables cumplen con la condición de hermiticidad,

460
00:37:40,130 --> 00:37:41,180
que es lo que les puse arriba.

461
00:37:42,040 --> 00:37:47,880
y las evoluciones temporales tienen que cumplir con la condición de unitariedad.

462
00:37:50,420 --> 00:37:55,500
También esto es como una especie de resumen de las propiedades de los sistemas cuánticos.

463
00:37:55,680 --> 00:38:00,420
Va, de las propiedades matemáticas que necesitan para representar a los sistemas cuánticos.

464
00:38:00,780 --> 00:38:02,780
Entonces ahora vamos a ver ejemplos de observables.

465
00:38:05,680 --> 00:38:07,560
Habíamos visto la vez pasada

466
00:38:12,280 --> 00:38:23,040
La habíamos visto que si uno tenía una fuente y tiraba en un campo magnético y ponía una

467
00:38:23,100 --> 00:38:31,560
pantalla al último, los átomos de plata se podían deflectar hacia arriba o hacia abajo

468
00:38:32,460 --> 00:38:36,880
y que la magnitud que estábamos midiendo en ese caso era lo que se conoce como el "spin",

469
00:38:36,880 --> 00:38:43,920
Bueno, entonces, y uno orienta al spin en la dirección zeta,

470
00:38:46,910 --> 00:38:51,740
si orientamos al, perdón, al imán en la dirección zeta, lo que vamos a hacer es un experimento

471
00:38:51,760 --> 00:38:57,440
para medir el spin en zeta. Entonces, medir el spin en zeta se va a representar por esta

472
00:38:57,500 --> 00:39:03,880
matriz que pongo acá. No estoy usando en este curso las constantes de físicas, no,

473
00:39:03,920 --> 00:39:07,320
no estoy usando la constante de Plan, nada acá, es todo adimensional.

474
00:39:07,940 --> 00:39:10,420
En un experimento real van a tener dimensiones,

475
00:39:10,660 --> 00:39:11,940
pero para no complicar las cosas,

476
00:39:12,880 --> 00:39:15,940
vamos a simplemente describir a los resultados

477
00:39:16,560 --> 00:39:19,100
del observable spin como para arriba y para abajo.

478
00:39:19,320 --> 00:39:21,380
Entonces ahí no necesitamos unidades físicas.

479
00:39:24,240 --> 00:39:25,760
Pero medir el spin en Z,

480
00:39:26,320 --> 00:39:28,780
créanme, va a estar representado por esta matriz de acá.

481
00:39:29,460 --> 00:39:33,200
Y esto es importante porque en la mayoría de las arquitecturas

482
00:39:33,200 --> 00:39:38,220
de computadoras cuánticas o en las arquitecturas de computadoras cuánticas más famosas que

483
00:39:38,280 --> 00:39:49,120
andan dando vuelta hoy por ahí, cuando realizan una medición siempre se hace con este observable,

484
00:39:49,520 --> 00:39:54,980
"spin z", ¿sí? Y en general uno va a tener que, déjenme escribir,

485
00:40:05,500 --> 00:40:12,140
uno va a tener que el 0 va a representar al valor 1 y el 1 va a representar al

486
00:40:12,160 --> 00:40:18,540
valor -1 del observable que se representa matemáticamente por esta

487
00:40:18,540 --> 00:40:24,580
matriz. Entonces cuando ustedes miden al qubit en lo que se conoce como base computacional

488
00:40:24,770 --> 00:40:33,520
que es esta base de acá, la base del 0, 1, esto lo vimos la vez pasada, ¿no? Esta se

489
00:40:33,580 --> 00:40:39,780
llama base computacional. Cuando miden a la computadora cuántica por default van a obtener

490
00:40:41,060 --> 00:40:47,740
1 y menos 1, ¿sí? Estos son los valores por default. En realidad, bueno, depende la

491
00:40:47,740 --> 00:40:55,100
convención que usen porque típicamente también podrían decir que es 0 o 1, pero bueno van a ver que eso en el fondo no es relevante.

492
00:40:55,160 --> 00:41:04,340
Entonces, estos son lo que se conoce como observables de spin. Este sigma z es medir el spin en la dirección z.

493
00:41:05,720 --> 00:41:14,180
Sigma i va a ser medir el spin en la dirección i. ¿Qué quiere decir eso? Bueno, que nosotros cuando tenemos la fuente,

494
00:41:16,539 --> 00:41:21,660
cuando tenemos la fuente que va a tirar el rayo de partículas, al campo magnético lo

495
00:41:21,700 --> 00:41:30,600
podemos orientar en distintas direcciones, x y z. Si medimos en la dirección y, si lo

496
00:41:30,640 --> 00:41:37,480
orientamos en la dirección y, vamos a estar midiendo este observable. Y por último, tenemos

497
00:41:37,640 --> 00:41:46,080
lo observable sigma x y esto quiere decir orientar al magneto en la dirección x, ¿tabian?

498
00:41:47,020 --> 00:41:52,600
la dirección z sería para arriba en la pantalla, la dirección x es pinchando así ustedes en

499
00:41:52,600 --> 00:41:58,940
la pantalla y la dirección y sería horizontal en la pantalla, ¿tabian? cada uno de esos

500
00:41:59,060 --> 00:42:03,600
experimentos es diferente, una cosa es medir el spin en x y otra cosa es medir el spin

501
00:42:03,600 --> 00:42:09,620
en z, que sé yo, no se puede medir el spin en las dos direcciones al mismo tiempo. O

502
00:42:09,660 --> 00:42:16,300
miden en x o miden en z, ¿por qué es así? Bueno, porque no pueden orientar un imán en

503
00:42:16,810 --> 00:42:21,760
tres direcciones distintas al mismo tiempo, o lo orientan en una dirección o lo orientan

504
00:42:21,760 --> 00:42:31,680
en la otra. Lo mismo con y, sí, son... Hacer experimento, medir en x, medir en y, y medir

505
00:42:31,680 --> 00:42:35,960
Y en Z representa a tres experimentos incompatibles entre sí.

506
00:42:36,100 --> 00:42:38,420
Son tres contextos de medición diferentes.

507
00:42:42,930 --> 00:42:45,340
Y estos tres contextos de medición diferentes están

508
00:42:45,420 --> 00:42:47,060
representados por estas tres matrices,

509
00:42:47,250 --> 00:42:48,340
que son todas distintas.

510
00:42:49,080 --> 00:42:52,940
Entonces ahora lo que les voy a explicar es cómo a partir de

511
00:42:52,940 --> 00:42:57,100
las matrices ustedes deducen los valores que puede tomar o no

512
00:42:57,160 --> 00:42:58,420
puede tomar el observable.

513
00:43:01,640 --> 00:43:05,820
Lo que va a terminar pasando es que los únicos valores que puede tomar

514
00:43:06,120 --> 00:43:10,680
este observable son 1 y -1 porque son los autobalores de la matriz,

515
00:43:11,310 --> 00:43:13,500
de la matriz de sigma x, sigma y y sigma z.

516
00:43:14,380 --> 00:43:17,800
Por ejemplo, si uno hace el experimento para medir en la dirección x,

517
00:43:17,850 --> 00:43:25,540
¿no? Entonces, los valores que va a tomar el observable cumplen con esta ecuación.

518
00:43:27,680 --> 00:43:32,840
y vamos a calcular ahora que lambda puede ser 1 o lambda puede ser igual a -1, ¿sí?

519
00:43:33,400 --> 00:43:35,100
Voy a hacer la cuenta en el pizarro.

520
00:43:38,220 --> 00:43:41,840
Lambda igual a 1 quiere decir que el el electrón se...

521
00:43:43,220 --> 00:43:46,000
el átomo se deflecta para arriba y lambda igual a -1

522
00:43:46,780 --> 00:43:48,600
quiere decir que se deflecta para abajo, ¿sí?

523
00:43:48,880 --> 00:43:49,880
1 y -1, ¿está bien?

524
00:43:50,440 --> 00:43:51,460
¿Hay una pregunta hasta ahora?

525
00:43:58,640 --> 00:44:09,440
Bien, sigo por acá. Bueno, decíamos, medir en x, medir en dirección x. Esto se representa

526
00:44:09,600 --> 00:44:16,000
matemáticamente por la matriz de Pauli, esta se conoce matriz de Pauli como sigma x, ¿no?

527
00:44:17,800 --> 00:44:20,400
Entonces, ¿qué valores puede tomar en X?

528
00:44:23,880 --> 00:44:29,640
Son los autovalores, lo que se conoce como autovalores de sigma X.

529
00:44:30,570 --> 00:44:33,520
Bueno, ¿cómo calculamos los autovalores de sigma X?

530
00:44:34,280 --> 00:44:41,820
Bien, necesito un vector, llamémosle B, distinto al vector nulo.

531
00:44:42,960 --> 00:44:50,940
este vector nulo es el que tiene 0,0, tal que exista un lambda que cumpla que

532
00:44:51,920 --> 00:44:57,740
sigma x por b se iguala lambda por b. Esta es la ecuación

533
00:45:00,900 --> 00:45:05,040
para los autovalores. Ahora vamos a ver cómo resolver esto.

534
00:45:05,200 --> 00:45:13,620
bueno, sigma x es, le escribo de vuelta, 0 1 1 0, un vector b para ser un alfabeta,

535
00:45:14,540 --> 00:45:22,180
porque b, este b es un vector de c2, son pares de números complejos,

536
00:45:23,600 --> 00:45:29,580
esto tiene que ser igual a lambda por alfabeta, pues voy a mostrar como calcular lambda,

537
00:45:32,300 --> 00:45:38,160
¿Cuánto vale lambda? ¿Cuánto tiene si esta es la matriz sin más de x? ¿Cuánto tiene

538
00:45:38,170 --> 00:45:43,240
que valer lambda para que exista un vector nonublo, es decir, una alfa beta para el cual

539
00:45:43,870 --> 00:45:49,080
no sea al mismo tiempo alfa y beta igual es a 0? Tal que esta matriz multiplicada por el

540
00:45:49,200 --> 00:45:54,760
vector es lo mismo que multiplicarla por un numerito lambda. Eso es lo que vamos a calcular

541
00:45:54,760 --> 00:46:01,560
a continuación, ok? Bien, entonces esto me define una ecuación, van a ver. Lo que primero

542
00:46:01,640 --> 00:46:07,580
voy a hacer, esto es, lo escribo de vuelta en términos de matrices y vectores, esto

543
00:46:07,620 --> 00:46:15,080
es sigma por b igual a lambda por b. Esto lo voy a pasar restando del otro lado, entonces

544
00:46:15,160 --> 00:46:23,060
esto es sigma x por b menos lambda por b igual a cero. Atención, este no es el cero de números,

545
00:46:23,400 --> 00:46:27,820
sino que es el 0 vector, es el 0 que tiene 0 coordenadas.

546
00:46:30,580 --> 00:46:44,760
Esto en este caso sería, en la parte de arriba sería 0 1 1 0 por alfa beta menos lambda por alfa beta y vala 0 0.

547
00:46:46,360 --> 00:46:52,420
Bien, ahora, ahora fíjense, en los dos términos de esta resta tengo a "b",

548
00:46:52,560 --> 00:46:59,620
¿sí? Entonces lo voy a sacar factor común a derecha, esto es lo mismo que sigma x menos

549
00:46:59,760 --> 00:47:07,840
lambda por la identidad por "b" igualado a 0. Ahora lo hago acá arriba, ¿no? Con los

550
00:47:07,880 --> 00:47:16,420
vectores, esto es 0,1,1,0 menos lambda por 1,001,

551
00:47:18,050 --> 00:47:19,280
con unos corchetes,

552
00:47:27,400 --> 00:47:32,880
pongo alfabet acá y esto tiene que ser igual al 0,0.

553
00:47:35,280 --> 00:47:48,080
Bien, bien, ahora esto es una matriz, llamémosle m, m por alfabeta igual a cero cero.

554
00:47:50,580 --> 00:47:56,960
¿Qué pasaría si m fuera inversible si existe m a la menos uno? ¿No? ¿Quién es la inversa de m?

555
00:47:57,020 --> 00:48:03,200
Bueno, m por m a la menos uno, si igual a la menos uno por m y esto da la identidad.

556
00:48:03,840 --> 00:48:10,520
¿Qué pasaría si existiera una matriz tal que es la inversa de M?

557
00:48:11,040 --> 00:48:17,000
Si existiera una matriz que es la inversa de M, esto debería dar alfa beta igual a M a la -1.

558
00:48:17,160 --> 00:48:20,500
Si paso la inversa del otro lado, ¿se entiende?

559
00:48:22,020 --> 00:48:28,040
Invierto la ecuación por 0, 0 y esto daría 0.

560
00:48:29,200 --> 00:48:31,980
Pero entonces alfa y beta tienen que ser si o si igual a 0.

561
00:48:32,440 --> 00:48:37,980
y esto no me sirve. ¿Por qué no me sirve? Porque por definición, para que tenga un

562
00:48:38,060 --> 00:48:42,800
autovector, el autovector tiene que ser distinto de cero, ¿sí? El b que estoy

563
00:48:42,860 --> 00:48:48,060
buscando acá tiene que ser distinto de cero. Entonces yo necesito que esta matriz

564
00:48:48,290 --> 00:48:56,160
m de acá, que es esto de acá, no sea inversible. Entonces hay un teorema que

565
00:48:56,160 --> 00:49:09,260
dice que m es inversible y sólo si el determinante de m es distinto del 0.

566
00:49:10,930 --> 00:49:16,540
Entonces yo no quiero que el determinante es una función, vamos a hacerlo para una matriz de 2 por 2,

567
00:49:16,640 --> 00:49:25,080
supongamos que m es igual a a b c d, el determinante de m es

568
00:49:27,760 --> 00:49:35,820
a por d menos b por c, ese es el determinante, es una cuenta muy sencilla, esta es la definición

569
00:49:35,820 --> 00:49:44,080
de determinante para una matriz de dos por dos, entonces la matriz es inversible si sólo

570
00:49:44,080 --> 00:49:49,220
sí, el determinante es distinto de 0. Entonces, yo no quiero que se inversible, porque quiero

571
00:49:49,340 --> 00:49:55,480
que este sistema de ecuaciones tenga una solución nonula, entonces tengo que pedir que el determinante

572
00:49:55,560 --> 00:50:06,280
de m sea igual a 0. Tiene que ser igual a 0. Eso es necesario para que existe este vector

573
00:50:06,390 --> 00:50:11,700
que llamaremos autovector. La solución de esto va a ser lo que se conoce como autovector.

574
00:50:12,320 --> 00:50:22,080
pregunta hasta acá a ver si no, esperen que si hay boli alguna pregunta como viene

575
00:50:22,080 --> 00:50:23,100
están muy perdidos

576
00:50:28,960 --> 00:50:29,160
bueno

577
00:50:30,560 --> 00:50:31,700
claro la de un autovector

578
00:50:32,960 --> 00:50:39,520
autovector claro si bueno lo digo lo digo más claro a ver

579
00:50:40,360 --> 00:50:41,340
vamos a ponerlo acá.

580
00:50:45,120 --> 00:50:46,480
B es

581
00:50:48,020 --> 00:50:48,700
autovector

582
00:50:51,500 --> 00:50:52,700
de una matriz A.

583
00:50:54,580 --> 00:50:59,200
Sí, se cumplen dos cosas. 1, B es distinto del vector nulo

584
00:51:00,470 --> 00:51:05,260
y 2 existe un número lambda complejo tal que

585
00:51:06,380 --> 00:51:08,900
A por B es igual a lambda por B.

586
00:51:10,460 --> 00:51:23,380
son dos condiciones, a es una matriz cuadrada de c a la n por n, entonces b va a ser autovector

587
00:51:23,780 --> 00:51:32,400
si b es no nulo y además existe un lambda, un numerito complejo tal que aplicarle a a

588
00:51:32,580 --> 00:51:38,880
b es decir multiplicar a por b es lo mismo que multiplicar a b por el número complejo lambda

589
00:51:41,220 --> 00:51:47,180
Sí, ahora sí. Bien, entonces esa es la definición, después lo que voy a hacer es en las diapositivas

590
00:51:47,340 --> 00:51:51,180
agrego la definición de autovector, porque ahora me voy a contar que está bueno que

591
00:51:51,180 --> 00:51:56,200
les quede ¿no? Una pregunta más allá de la definición formal, conceptualmente ¿qué

592
00:51:56,440 --> 00:52:06,280
sería? Ah bueno, perdón, y lambda es autovalor. Entonces,

593
00:52:07,640 --> 00:52:13,060
es que existe un lambda tal que a por b es lambda por b y autovalor es el lambda

594
00:52:13,740 --> 00:52:16,220
tiene que existir un b tal que a por b sea lambda por b.

595
00:52:17,600 --> 00:52:22,880
Entonces en este caso b sería un auto vector da de autovalor lambda

596
00:52:23,300 --> 00:52:28,240
en este caso. Ahora vamos a calcular los autoactores y autovalores de sigma x.

597
00:52:29,040 --> 00:52:34,360
Bien, intuitivamente ¿qué sería? buena pregunta. Volvamos a esta ecuación.

598
00:52:34,440 --> 00:52:41,640
a por b es igual a lambda por b. Supongamos que la matriz es real, no? Supongo que tengo

599
00:52:41,640 --> 00:52:54,380
una matriz que a por el 1, 1 es igual a 2 por 1, 1. Esta sería una matriz que viene al

600
00:52:54,460 --> 00:53:03,600
1, 1 como autovector de autovalor 2. Entonces, si el 1, 1 es este, ¿qué quiere decir esto?

601
00:53:03,800 --> 00:53:07,580
si definís la transformación lineal, ¿te acuerdas que decíamos? Si defino la

602
00:53:07,760 --> 00:53:17,440
transformación f suba de 1 1 es 2 por 1 1, es decir, son vectores tales que para

603
00:53:17,440 --> 00:53:23,640
la transformación lineal que define la matriz A, para esos vectores la

604
00:53:23,680 --> 00:53:28,360
transformación lineal se reduce a multiplicar por lambda, ¿me se dice?

605
00:53:30,520 --> 00:53:36,420
en este caso multiplicar por 2, si vos aplicas a a cualquier otro vector no va a

606
00:53:36,560 --> 00:53:39,360
ser necesariamente multiplicar por 2, ¿entendés?

607
00:53:44,200 --> 00:53:45,400
¿Podrás repetir esto último por favor?

608
00:53:46,150 --> 00:53:56,980
Si, vos podréis definir una transformación lineal muy sencilla, una f tal que f de b es igual a 3 por b, ¿entendés?

609
00:53:57,660 --> 00:54:01,700
para todo. Esta es una transformación lineal.

610
00:54:05,320 --> 00:54:10,440
Sin embargo, no es cierto que todas las transformaciones lineales sean así.

611
00:54:10,980 --> 00:54:13,080
Esta es una transformación lineal muy sencilla.

612
00:54:15,500 --> 00:54:22,620
En general, por ejemplo, habíamos visto, la vez pasada, que si ya sea, coseno de tita,

613
00:54:25,020 --> 00:54:25,580
"Tito"

614
00:54:28,280 --> 00:54:30,000
"Tito" creo que era así ¿no?

615
00:54:30,160 --> 00:54:31,560
"Coceno" no...

616
00:54:31,720 --> 00:54:32,860
"Coceno Tito"

617
00:54:35,160 --> 00:54:35,800
¿Cómo era?

618
00:54:36,800 --> 00:54:39,100
¿Había una que era una rotación en tita? ¿te acordás?

619
00:54:39,240 --> 00:54:40,260
La vimos la vez pasada

620
00:54:42,540 --> 00:54:45,520
Lo que hacía la rotación era rotar un vector

621
00:54:45,720 --> 00:54:47,020
Esta era una transformación lineal

622
00:54:48,500 --> 00:54:51,080
Me la rotaba un ángulo que es yo... tita, ¿sí?

623
00:54:52,820 --> 00:54:54,660
la transformación era rotar.

624
00:54:58,320 --> 00:54:59,520
¿Cómo debería ser?

625
00:55:00,260 --> 00:55:00,780
Está claro.

626
00:55:01,260 --> 00:55:04,340
Entonces esa no multiplica a los vectores por un número.

627
00:55:04,720 --> 00:55:05,100
¿Entendés?

628
00:55:06,640 --> 00:55:07,100
Sí.

629
00:55:10,260 --> 00:55:14,780
Vos lo que estás diciendo cuando decís que B es que el ámbito es autovector,

630
00:55:15,060 --> 00:55:17,240
es que A por B,

631
00:55:18,380 --> 00:55:19,860
aplicarle A a B,

632
00:55:20,160 --> 00:55:26,660
es lo mismo que multiplicar a b por un numerito lambda y eso no va a pasar para todos los vectores, ¿me entendés?

633
00:55:27,280 --> 00:55:31,640
O sea, el ejemplo de la rotación no sería un autovalor.

634
00:55:31,640 --> 00:55:32,920
Claro, no es un autovalor.

635
00:55:34,720 --> 00:55:45,020
No, algo que es, si, depende porque si r0, si tita es 180 grados suponete, a un b lo pasas a -b,

636
00:55:45,100 --> 00:55:50,220
Entonces es autovector de autovalor -1, ¿no?

637
00:55:50,420 --> 00:55:50,800
¿Entendés?

638
00:55:51,520 --> 00:55:51,620
Sí.

639
00:55:51,820 --> 00:55:59,860
Pero en general, que si yo así roto a 45 grados, el B no es autovector porque no es un múltiplo.

640
00:56:00,200 --> 00:56:06,300
Para ser autovector, la aplicación de la transformación lineal tiene que ser un múltiplo, ¿no entendés?

641
00:56:08,480 --> 00:56:09,520
Sí, sí, sí, gracias.

642
00:56:10,520 --> 00:56:15,780
Bien, esa es la interpretación geométrica, pero para nosotros la interpretación va a ser que

643
00:56:17,180 --> 00:56:22,860
los autobalores son los valores que puede tomar el observable en consideración, ¿entendés?

644
00:56:24,460 --> 00:56:31,100
Entonces, volviendo, ¿no? Volviendo a sigma x, repito las cuentas, sigma x será 0 1 1 0,

645
00:56:31,100 --> 00:56:38,320
entonces hacíamos 0 1 1 0 por alfabeta igual a lambda por alfabeta

646
00:56:40,360 --> 00:56:45,140
esta es la ecuación, quiero buscar el lambda tal que es auto vector

647
00:56:46,580 --> 00:56:56,460
entonces paso restando y me queda 0 1 1 0 por alfabeta menos lambda por alfabeta igual al 0 0

648
00:56:58,320 --> 00:57:05,980
Ahora saco factor común el alfabeto, entonces me queda 0 1 1 0 menos lambda por 1 0 0 1, la identidad

649
00:57:08,420 --> 00:57:16,480
por alfabeto igual a 0 0. Bueno ejercicio y recontre ejercicio que tienen que hacer en sus casas es repetir

650
00:57:16,560 --> 00:57:22,660
estas cuentas. Esto es un ejercicio básico de alfgelalínal que es calcular

651
00:57:22,660 --> 00:57:30,000
auto vectores y auto valores de una matriz. Bien, entonces ahora sigo con las cuentas. Esto lo

652
00:57:30,040 --> 00:57:40,760
junto todo y me queda. Primero 0 1 1 0 menos, tengo que multiplicar a cada uno de los componentes por

653
00:57:40,780 --> 00:57:54,540
lambda lambda 0 0 lambda por alfa beta igual a 0 0, si va abajo, me queda menos lambda 1

654
00:57:54,560 --> 00:58:00,640
menos 0 1 1 menos 0 1 0 menos lambda menos lambda por alfa beta igual a 0.

655
00:58:02,500 --> 00:58:10,220
Entonces yo quiero, yo quiero que esto tenga soluciones no nulas, yo quiero que exista

656
00:58:10,220 --> 00:58:12,640
una alfa y beta que sea distinto de cero, ¿por qué?

657
00:58:13,120 --> 00:58:15,120
Bueno, porque es la condición para hacer auto vector,

658
00:58:15,460 --> 00:58:18,340
el B tiene que ser distinto del vector nulo.

659
00:58:19,320 --> 00:58:22,720
Entonces, para eso tengo que pedir que el determinante de esta matriz,

660
00:58:25,820 --> 00:58:29,640
el determinante de -lambda 1, 1 -lambda,

661
00:58:30,180 --> 00:58:30,840
sea igual a cero.

662
00:58:32,060 --> 00:58:34,960
Bien, el determinante es este por este,

663
00:58:36,200 --> 00:58:38,300
menos este por este, si entonces es,

664
00:58:38,780 --> 00:58:48,280
menos lambda por menos lambda, menos 1 por 1 igual a 0, menos lambda por menos lambda es

665
00:58:48,340 --> 00:58:54,860
lambda cuadrado, 1 por 1 es 1, y acá me sale que cuando despejo esto me queda lambda cuadrado

666
00:58:54,920 --> 00:59:00,500
igual a 1 y las dos soluciones de esta ecuación son lambda igual a 1 y lambda igual a menos

667
00:59:00,680 --> 00:59:05,620
1. ¿Qué quiere decir esto físicamente más allá de la interpretación geométrica que

668
00:59:05,620 --> 00:59:12,860
discutimos recién con Emiliano, lo que quiere decir físicamente es que la matriz sigma x

669
00:59:13,430 --> 00:59:20,260
que representa el observable físico medir el spin en la dirección x, puede tomar solo

670
00:59:20,270 --> 00:59:26,260
dos valores, de si sea un experimento de medir el spin en la dirección x, puede valer o 1

671
00:59:26,540 --> 00:59:27,620
o -1, ¿sí?

672
00:59:28,640 --> 00:59:31,720
Esas son las únicas dos posibilidades que tengo. ¿Está bien?

673
00:59:35,720 --> 00:59:37,400
Esa es la primera cosa, ¿sí?

674
00:59:39,860 --> 00:59:41,680
¿Y eso qué significa?

675
00:59:42,600 --> 00:59:48,640
Que si yo tiro el rayo, tengo la fuente, tiro el rayo, le pongo el imán en la dirección "x",

676
00:59:50,220 --> 00:59:54,540
entonces el rayo se puede deflectar para arriba o para abajo en la dirección "x".

677
00:59:54,540 --> 01:00:00,020
si se representa para arriba dio una y si se deflecta para abajo dio menos uno.

678
01:00:00,850 --> 01:00:06,040
¿Se entiende esto? ¿Alguna pregunta? No tiene nada que ver con su posición.

679
01:00:07,800 --> 01:00:12,360
Bueno, todavía no, pero pronto sí. Este ejemplo concreto que hice del

680
01:00:12,420 --> 01:00:16,400
rayo con el imán no sería su posición eso o va para un lado o va para el otro.

681
01:00:17,380 --> 01:00:23,360
No, sí, sí, va a haber superposición porque hará la gracia sexta.

682
01:00:24,220 --> 01:00:33,860
Yo ahora, por ejemplo, podría preparar a mi sistema en este estado, en el arriba en z,

683
01:00:34,960 --> 01:00:39,820
1/2/2 por arriba en z menos 1/2/2 por abajo en z, ¿sí?

684
01:00:40,460 --> 01:00:41,400
en la dirección z.

685
01:00:46,740 --> 01:00:47,620
Esto sería...

686
01:00:47,640 --> 01:00:48,960
Sí, bueno, en este estado, ¿no?

687
01:00:49,480 --> 01:00:52,940
¿Qué pasa si ahora, mido en la dirección x?

688
01:00:54,640 --> 01:00:58,320
Yo tiro el rayo en este estado obsidio de arriba, ¿sí?

689
01:00:59,660 --> 01:01:02,380
¿Qué pasa si ahora, mido el spin en la dirección x?

690
01:01:10,000 --> 01:01:10,440
Bueno...

691
01:01:10,440 --> 01:01:15,140
este ahora vamos a ver lo que pasa con este déjenme hacer la cuenta de los

692
01:01:15,240 --> 01:01:25,180
autovectores del spin. Vos podrías armar por ejemplo un phi que sea uno sobre

693
01:01:25,420 --> 01:01:34,920
raíz de 2 por arriba en x menos uno sobre raíz de 2 por abajo en x y ahí tenés una

694
01:01:35,000 --> 01:01:40,420
superposición ¿entendés? Si vos ahora midieras el spin en x tendrías que con una

695
01:01:40,420 --> 01:01:45,240
cierta probabilidad se va para arriba o para abajo. Pero vos no tenés que confundir probabilidades

696
01:01:45,270 --> 01:01:53,260
con autobelores. Los autobalores son los posibles valores que puedes llegar a tomar tu observable

697
01:01:53,450 --> 01:02:02,920
en un experimento. Y otra cosa es la probabilidad con la cual salen estos dos valores. ¿Entendés

698
01:02:03,020 --> 01:02:10,880
son dos cosas distintas, es como que yo te diga tengo un dado, tengo un dado. El dado puede tomar

699
01:02:11,150 --> 01:02:20,320
seis valores posibles, sí? Bueno, esos serían los autobalores, ¿entendés? Ahora, cuando yo hago

700
01:02:20,320 --> 01:02:27,560
un experimento concreto con mi dado, puede salir cualquiera de esos autobalores con alguna probabilidad,

701
01:02:27,560 --> 01:02:36,380
la probabilidad va a venir dada con el estado. Una cosa es el observable. Cima x es el observable.

702
01:02:39,260 --> 01:02:44,720
Y el observable ya me dice que solo puede tomar valores 1 y -1.

703
01:02:47,260 --> 01:02:51,920
Esos son los únicos dos valores que puede tomar. Bueno, cuando haga un experimento concreto,

704
01:02:51,960 --> 01:03:00,820
el resultado va a depender no sólo del observable sino del estado. El estado sí me va a dar la

705
01:03:00,880 --> 01:03:04,680
probabilidad con la que sale 1 y la probabilidad con la que sale -1, ¿me entendés?

706
01:03:10,240 --> 01:03:14,940
Son dos cosas conceptualmente distintas. El observable es como que yo te diría

707
01:03:16,760 --> 01:03:21,400
¿Cuánto puede valer la energía de un sistema? Bueno, tal rango de valores, ¿me

708
01:03:21,480 --> 01:03:28,720
entiendes? ¿o cuantos cuáles pueden ser los resultados del lado? Bueno, 1, 2, 3, 4, 5, 6,

709
01:03:28,920 --> 01:03:34,380
esos tenían como los autobalores. Ahora, cuando yo preparo el lado en un estado,

710
01:03:35,380 --> 01:03:42,140
le asigno probabilidades a cada uno de esos valores, ¿me entiendes? Y cuando el experimento,

711
01:03:42,140 --> 01:03:49,900
las frecuencias que observen el laboratorio van a ser, se van a aparecer a esas probabilidades,

712
01:03:50,220 --> 01:03:59,880
¿entendés? -Sí. -Bien, sigo, entonces lo que logramos con esto, sí. -Sí, disculpe,

713
01:04:00,280 --> 01:04:06,140
¿puedo volver a explicar la parte de auto-vector? Porque la parte de auto-valor la acabo de entender con lo que

714
01:04:06,140 --> 01:04:15,260
-Explico de... -No, claro, claro, ahora voy al autodector. Volvamos, volvamos a esto. ¿Te acordás de esto?

715
01:04:16,460 --> 01:04:19,680
-Sí. -Volvamos a esto. Acá, ¿qué hacía yo?

716
01:04:20,440 --> 01:04:25,480
Estaba calculando los autovalores, ¿no? Y me salió que eran 1 y -1, ¿sí? Hasta acá.

717
01:04:29,040 --> 01:04:33,220
En toda esta línea de razonamiento, ¿no? ¡Psh! Flecha para acá.

718
01:04:33,220 --> 01:04:41,620
yo calculé que los autobalores de sigma x eran 1 menos 1 con esta técnica. Es una técnica en

719
01:04:41,660 --> 01:04:47,440
cualquier libro de álgel a lineal vas a encontrar esta cuenta de alguna manera u otra. Entonces yo

720
01:04:47,440 --> 01:04:53,800
lo que les recomiendo es, sigan leyendo el libro de Daniel Senechang y sigan viendo todo esto.

721
01:04:54,859 --> 01:04:59,760
usé un ejemplo. Bien, ahora que calculamos los autovalores vamos a

722
01:04:59,780 --> 01:05:07,440
calcular los autovectores. Ok, porque qué era un autovector de sigma x? Un autovector era

723
01:05:07,540 --> 01:05:16,540
un v tal que sigma v es 1 por v o sigma x por v es igual a -1 por v ¿Estás de acuerdo?

724
01:05:16,680 --> 01:05:18,500
esta es la definición de autovector

725
01:05:21,120 --> 01:05:27,360
¿por qué puse -1? esto era sigma x por b igual a lambda por b pero vimos que lambda

726
01:05:27,460 --> 01:05:30,400
era igual a 1 o lambda igual a -1

727
01:05:33,000 --> 01:05:37,700
lo acabamos de ver entonces ahora vamos a ir a buscar a ver quién es este b

728
01:05:38,120 --> 01:05:43,520
ok vamos a calcularlo te voy a enseñar a calcularlo bien entonces volvamos a

729
01:05:43,520 --> 01:05:49,400
esta ecuación, pues vamos a hacer esta ecuación de arriba. Yo tenía, volvamos ¿no?

730
01:05:49,680 --> 01:05:56,620
Lo vuelvo a escribir para que sea más fácil. Yo tenía 0 1 1 0 ¿no? que era sigma x por

731
01:05:58,420 --> 01:06:06,920
alfabeta igual a lambda por alfabeta. Pero ya vimos que lambda era 1 o lambda era igual

732
01:06:06,920 --> 01:06:12,320
menos 1, bueno, elijamos lambda igual a 1, primero vamos a resolver

733
01:06:13,000 --> 01:06:18,340
autodictores para lambda igual a 1, si lambda es 1 tengo 0 1 1 0, alfabeta que

734
01:06:18,360 --> 01:06:24,480
todavía no sé quiénes son, por 1 por alfabeta, bueno pero 1 por alfabeta es alfabeta

735
01:06:25,880 --> 01:06:35,400
entonces solo paso restando y me queda 0 1 1 0 por alfabeta, perdón, menos alfabeta

736
01:06:36,040 --> 01:06:40,340
y vale al 0,0 y esto es

737
01:06:43,740 --> 01:06:49,840
saco factor del alfabeto 0,1,1,0, lo hago muy lento esto, perdón para los que ya lo

738
01:06:49,980 --> 01:06:59,540
sepan, menos 1,0,0,1 por alfabeto y vale a 0, los que ya hayan tomado un curso

739
01:06:59,740 --> 01:07:02,400
del eje berenil y de matemática van a ver que acá me va a querer un sistema de

740
01:07:02,400 --> 01:07:19,200
ecuaciones. Entonces esto me queda -1, 1, 1, -1 por alfa beta igual a 0,0. Bien, multiplico,

741
01:07:19,520 --> 01:07:26,220
hago la cuenta, tengo multiplicar, multiplicación matricial me queda, menos alfa más beta en

742
01:07:26,220 --> 01:07:31,119
la primera coordenada y alfa menos beta en la segunda coordenada, esto tiene que ser igual

743
01:07:31,120 --> 01:07:40,780
0 a 0. Entonces de la primera saco que -alpha + beta es igual a 0 y de la segunda saco que

744
01:07:40,880 --> 01:07:47,740
alfa -beta es igual a 0, con lo cual alfa es igual a beta en las dos, de las dos me sale que alfa

745
01:07:47,800 --> 01:07:57,840
es igual a beta. Entonces recapitulando, para lambda y o ala 1, para león de o ala 1, los alfa beta

746
01:07:57,840 --> 01:08:04,840
que busco cumplen que alfa es igual a beta. Entonces acá pongo alfa y acá pongo alfa.

747
01:08:06,300 --> 01:08:13,440
Entonces los alfa-betas que busco son de la forma alfa-alfa, que es alfa por uno uno.

748
01:08:14,700 --> 01:08:21,040
Entonces lo que me queda es que los autobectos... ¿cuántos pregunto? ¿cuántos autobectores encontré?

749
01:08:23,000 --> 01:08:23,720
infinitos.

750
01:08:24,940 --> 01:08:27,279
Infinitos, porque para cada valor de alfa,

751
01:08:27,380 --> 01:08:29,740
acá alfa pertenece a complejos.

752
01:08:30,980 --> 01:08:33,980
Cada valor de alfa me va a definir un autovector distinto,

753
01:08:34,100 --> 01:08:38,680
porque cualquier vector de la forma alfa-alfa me sirve como

754
01:08:39,000 --> 01:08:40,400
autovector de autovalor 1.

755
01:08:41,160 --> 01:08:42,819
Entonces, por ejemplo, hagámosla cuenta, ¿no?

756
01:08:43,779 --> 01:08:45,060
Sigma x por 1, 1.

757
01:08:46,299 --> 01:08:50,220
Debo hacer 0, 1, 1, 0 por 1, 1.

758
01:08:51,319 --> 01:08:59,520
¿Cuánto me va a dar? 1, 1, me tiene que dar. No, 1, 1, me tiene que dar. 1, 1, porque es un

759
01:08:59,860 --> 01:09:07,740
autovector de autovalor 1, ¿entendés? Y si ahora hago 2 por 1, 1, hago sigma x por 2, 2, ¿no?

760
01:09:07,900 --> 01:09:16,960
¿Cuánto me va a dar? Igual, ¿entendés? 0, 1, 1, 0 por el 2, 2. Me queda 2, 2, ¿sí? Porque son

761
01:09:16,960 --> 01:09:24,880
todos autodectores de autovalor 1. Bueno, tan importante es el... lo copio de vuelta, ¿no?

762
01:09:28,920 --> 01:09:35,980
Hacemos sigma x por 1,1 igual a 1,1, dijimos, ¿no? Bien, hay uno que es muy importante,

763
01:09:36,259 --> 01:09:47,220
es este, si hago el vector 1, 1, si considero este vector, la norma de este vector es 2,

764
01:09:47,380 --> 01:09:55,320
es si, raíz de 2, porque es raíz de 1 al cuadrado más 1 al cuadrado, eso es raíz de

765
01:09:56,440 --> 01:10:07,380
Entonces me voy a armar el vector si sabemos le si 1x igual a 1 sobre raíz de 2 por 1,1.

766
01:10:08,880 --> 01:10:14,420
Entonces acá el alfa es igual a 1 sobre raíz de 2. Entonces este también es

767
01:10:14,500 --> 01:10:19,880
autovector de autóvalor 1, pero la virtud de este vector se los dejo como ejercicio

768
01:10:19,880 --> 01:10:29,040
pero haces la cuenta que la norma de phi 1x es igual a 1, la norma es 1, bien pero

769
01:10:29,100 --> 01:10:40,360
¿quién es phi 1x? si 1x es 1 sobre raíz de 2, 1 sobre raíz de 2 y esto es lo mismo

770
01:10:40,460 --> 01:10:56,780
que 1/√2 por 1,0 más 1/√2 por 0,1. Si llamamos al 0, le llamamos 1,0 y al 1 le llamamos 0,1,

771
01:10:58,740 --> 01:11:03,740
este vector es 1 a raíz de 2 por 0 más 1, ok?

772
01:11:07,500 --> 01:11:12,860
y este vector es importante en común, si os contigo que se llama más, lo vamos a llamar

773
01:11:12,900 --> 01:11:13,480
así, ok?

774
01:11:14,880 --> 01:11:28,720
recuerden que esta era la base computacional, el 1, 0 y el 0, 1 eran lo que formaba la base

775
01:11:28,720 --> 01:11:32,880
ahora sí, me había preguntado, creo que Leandro, esta es una superposición, ¿entendés?

776
01:11:34,080 --> 01:11:40,900
el más es una superposición, pero el 0, 1, ¿en qué base? en la base computacional,

777
01:11:41,200 --> 01:11:51,200
el más que sería autovector de autovalor 1 de sin más de x, ay, perdón, yo le puse

778
01:11:51,280 --> 01:11:57,560
acá x y no quise poner, quise poner más. Sigma x por más es uno por más.

779
01:12:01,239 --> 01:12:07,580
Este tiene norma 1 con lo cual podría representar un estado cuántico. ¿Qué estado cuántico?

780
01:12:07,640 --> 01:12:12,380
Bueno, un estado que es la superposición entre 0 y 1. Es un estado que es

781
01:12:13,360 --> 01:12:18,280
superposición equiprobable en la base computacional. Entonces, este no solo es

782
01:12:18,280 --> 01:12:24,760
auto vector sino que también es un auto estado de sigma x. ¿Qué quiere decir eso?

783
01:12:24,860 --> 01:12:29,140
Bueno, que si ustedes preparan, supongamos que preparamos el rayo cuántico, ¿no?

784
01:12:30,900 --> 01:12:40,380
En el estado más, cuando yo mida a una medición del spin en la dirección x, me va a dar

785
01:12:40,400 --> 01:12:50,820
con probabilidad 1 + 1 y con probabilidad 0 el -1. Ahora si a este mismo estado, a este

786
01:12:50,940 --> 01:12:59,980
mismo estado, le mido el spin, si preparo en la dirección más y mido el spin en z,

787
01:13:02,440 --> 01:13:09,080
voy a tener con probabilidad 1/2 1 y con probabilidad 1/2 -1, eso lo vamos a calcular después,

788
01:13:09,160 --> 01:13:13,500
pero esa es la idea, por eso son todas cosas distintas, una cosa son los

789
01:13:13,620 --> 01:13:20,060
autobalores, que son los valores posibles que podría tomar una observable en

790
01:13:20,140 --> 01:13:25,360
una experimenta. Los autobalores se calculan como les dije, son los lambda

791
01:13:25,460 --> 01:13:34,560
tal que a por b es igual a lambda por b donde b es distinto de 0, así calculan

792
01:13:34,560 --> 01:13:36,980
los valores posibles que podría ya tomar un observable.

793
01:13:38,960 --> 01:13:40,240
Luego hay autostados.

794
01:13:40,580 --> 01:13:44,000
Los autostados son tales que, si hacen una medición en ese

795
01:13:44,080 --> 01:13:48,120
autostado, le da con seguridad el autovalor asociado a ese

796
01:13:48,200 --> 01:13:49,020
autostado.

797
01:13:50,580 --> 01:13:53,120
Y después, otra cosa distinta es el estado,

798
01:13:53,300 --> 01:13:54,800
el estado general del sistema.

799
01:13:56,300 --> 01:14:01,600
El estado general del sistema podría ser un autostado del

800
01:14:01,680 --> 01:14:03,600
observable que están viendo o no.

801
01:14:04,520 --> 01:14:09,600
¿Podrá hacerlo o no? Bueno, si lo es, pasa una cosa y si no lo es, pasa otro.

802
01:14:09,730 --> 01:14:12,020
¿Tá bien? Pero eso lo vamos sirviendo después.

803
01:14:14,460 --> 01:14:18,400
Bueno, veamos otro. Les había dicho que teníamos, ¿no?

804
01:14:19,500 --> 01:14:25,020
Distintos, está, "medir en X", "medir en I". Bueno, les dejo a ustedes como ejercicio

805
01:14:27,559 --> 01:14:36,300
calcular los autobalores y autovectores del spineni. También les va a dar que los

806
01:14:36,400 --> 01:14:43,180
lambda son 1 y -1. En este caso, pero tienen que hacer lo mismo. Es importante

807
01:14:43,270 --> 01:14:48,560
que lo hagan ustedes en sus casas. Calcular autobalores y autovectores del

808
01:14:48,660 --> 01:14:54,840
spineni. Y la otra cosa que acá nos faltó calcular, yo calculé los

809
01:14:54,840 --> 01:14:57,620
los auto vectores para lambda igual a 1 ¿se acuerdan?

810
01:14:58,960 --> 01:15:02,460
perten que vuelvo al... tengo que seccionar algo acá

811
01:15:03,480 --> 01:15:06,640
para lambda igual a 1, hicimos toda la cuenta

812
01:15:06,880 --> 01:15:12,520
y me quedo que los auto vectores serán de la forma

813
01:15:12,900 --> 01:15:15,580
alpha por 1 a 1, ahora hagamos todo lo mismo para

814
01:15:16,460 --> 01:15:20,840
lambda igual a -1, vamos a ver qué pasa

815
01:15:20,840 --> 01:15:22,500
¿Lando o no? -1

816
01:15:50,840 --> 01:15:59,740
de la empresa con factor común menos más, perdón, más 1, 0, 0, 1 por topo por alfa,

817
01:15:59,920 --> 01:16:03,060
beta, igual a 0, 0.

818
01:16:05,260 --> 01:16:10,800
Ahora que esta matriz, 1, 1, 1, 1 por alfa, beta, igual a 0, 0.

819
01:16:12,700 --> 01:16:18,739
Cuando despejan, les quedan que alfa más beta tiene que igual, ser igual a 0, entonces

820
01:16:18,740 --> 01:16:26,000
alfa tiene que ser igual a -beta. Entonces, para lambda igual a -1, lo que termina pasando

821
01:16:26,320 --> 01:16:35,960
es que los alfa-beta que buscamos, si pongo alfa-k, acá tengo que poner -alpha. Entonces,

822
01:16:36,240 --> 01:16:45,020
son todos múltiplos del 1-1. ¿Qué quiere decir eso? Bueno, que de nuevo, si yo hago

823
01:16:45,020 --> 01:16:51,360
Sigma x que es 0, 1, 1, 0 por 1, -1, 1, -1, ¿cuánto me va a dar?

824
01:16:52,380 --> 01:16:56,780
Que me lo digo al 1, a ver al 1 si está atento. ¿Cuánto tiene que dar?

825
01:16:58,220 --> 01:16:59,080
1, -1.

826
01:17:01,280 --> 01:17:03,100
Tiene que dar -1, 1.

827
01:17:04,320 --> 01:17:10,300
Cambio del signo ¿por qué? ¿Por qué este es autovector de autovalor -1?

828
01:17:11,120 --> 01:17:13,680
es decir, este se multiplica por -1, ¿entienden?

829
01:17:13,760 --> 01:17:16,100
Y haz la cuenta, 0 por -1, ¿sabe?

830
01:17:18,720 --> 01:17:20,420
Háganlo en sus casas, esto de vuelta,

831
01:17:20,940 --> 01:17:22,200
convénsense que esto es así.

832
01:17:23,200 --> 01:17:23,440
¿Está bien?

833
01:17:24,480 --> 01:17:29,260
Que esto es -1 por 1 -1, ¿sí?

834
01:17:31,620 --> 01:17:34,260
¿Por qué? Porque es autovector de autovalor -1.

835
01:17:35,260 --> 01:17:39,460
Y bueno, de vuelta, cuando dan la norma de si llaman b

836
01:17:39,460 --> 01:17:46,640
igual a 1 menos 1, la norma de B les da 2, perdón, raíz de 2,

837
01:17:48,220 --> 01:17:53,860
entonces si dividen, se hacen 1 sobre raíz de 2 por B,

838
01:17:54,260 --> 01:18:00,640
esto se llama en la literatura menos, les queda el 1 sobre raíz de 2 por 0,

839
01:18:00,820 --> 01:18:03,080
menos 1 sobre raíz de 2 por 1.

840
01:18:05,760 --> 01:18:11,320
y B' que es el más que definimos arriba y el menos,

841
01:18:11,580 --> 01:18:15,040
es una base alternativa a la base computacional B.

842
01:18:18,520 --> 01:18:23,840
Como base del espacio vectorial de un qubit pueden usar B' o B.

843
01:18:24,360 --> 01:18:27,580
Esta sería la base que tiene más y menos.

844
01:18:28,180 --> 01:18:34,039
En general, los autovectores de un observable sin degeneración

845
01:18:34,640 --> 01:18:39,460
van a dar lugar a una base del espacio vectorial.

846
01:18:41,560 --> 01:18:43,580
Y hacen la cuenta, ah bueno, todavía no lo expliqué,

847
01:18:43,760 --> 01:18:47,100
pero van a ser ortogonales, van a tener ángulo 90 grados.

848
01:18:47,220 --> 01:18:48,720
¿Sí? Bueno, hay una pregunta con esto.

849
01:18:56,660 --> 01:19:00,440
Bueno, y como ejercicio escribir al cero

850
01:19:05,020 --> 01:19:09,040
¿Cómo se escribe 0 en términos de alpha más beta por menos?

851
01:19:09,570 --> 01:19:15,840
Si esto es una base tiene que generar, entonces tienen que poder hacer esto y tienen que poder escribir al 1 como...

852
01:19:18,520 --> 01:19:21,700
Bueno, eso se los dejo como ejercicio, ¿sí? Hagan esto.

853
01:19:23,700 --> 01:19:26,980
Es importante y es fácil al mismo tiempo. Así que esto lo tienen que poder hacer.

854
01:19:28,040 --> 01:19:29,200
Si no le sale, me preguntan.

855
01:19:31,260 --> 01:19:31,480
Bien.

856
01:19:35,720 --> 01:19:39,220
Entonces ahí les mostré cómo calcular autovactores y

857
01:19:39,240 --> 01:19:41,680
autovalores de matrices.

858
01:19:42,060 --> 01:19:44,580
Con estos ejemplos, como ejercicio,

859
01:19:44,640 --> 01:19:47,320
tienen que calcular acá.

860
01:19:47,660 --> 01:19:53,540
Entonces lo que van a encontrar cuando van el de sigma zeta es

861
01:19:53,540 --> 01:19:57,940
que para sigma zeta también lambda es igual a 1 o lambda es

862
01:19:58,000 --> 01:19:58,760
igual a -1.

863
01:19:59,340 --> 01:20:04,800
y los autostados son 0 y 1.

864
01:20:06,380 --> 01:20:11,420
Entonces, 0 va a ser autoestado de lambda igual a 1 para sigma zeta

865
01:20:11,520 --> 01:20:15,660
y 1 va a ser autoestado de lambda igual a -1 para sigma zeta.

866
01:20:16,140 --> 01:20:19,980
Entonces, cuando tengan una computadora cuántica para fijar ideas,

867
01:20:20,100 --> 01:20:20,960
pueden pensar en eso.

868
01:20:21,680 --> 01:20:25,020
Pueden pensar que si miden al qubit en la base computacional,

869
01:20:25,260 --> 01:20:27,099
lo que están haciendo es medir sigma zeta

870
01:20:28,100 --> 01:20:33,800
y para fijar ideas pueden pensar en que orientan al magneto en la dirección z.

871
01:20:34,580 --> 01:20:40,960
Entonces, si obtienen 1, quiere decir que obtuvieron 0 y si obtienen -1,

872
01:20:41,380 --> 01:20:42,520
quiere decir que obtuvieron 1.

873
01:20:45,220 --> 01:20:46,500
Atención, atención.

874
01:20:47,480 --> 01:20:54,480
Esto no quiere decir que todas las computadoras cuánticas se puedan pensar como un átomo

875
01:20:54,480 --> 01:20:58,900
que atraviesa por un imán y se deflecta el rayo para arriba o para abajo.

876
01:20:59,040 --> 01:21:03,260
No, para nada, porque no es así, físicamente no es así.

877
01:21:03,780 --> 01:21:07,160
Pero es una forma de representarlo, va a haber muchas instanciaciones

878
01:21:07,950 --> 01:21:12,180
de sistema físico para los cuales Sigma Z es uno observable

879
01:21:12,550 --> 01:21:15,200
y los autovalores y autovectores son estos, ¿ok?

880
01:21:15,710 --> 01:21:18,840
Y así va a ser en la mayoría de las arquitecturas de computadoras cuánticas.

881
01:21:20,080 --> 01:21:30,760
Entonces, esto les tiene que servir para poder tener una mínima representación física de la matemática que estamos utilizando aquí, ¿OK?

882
01:21:31,860 --> 01:21:32,020
Bien.

883
01:21:33,480 --> 01:21:35,900
Bueno, son y media.

884
01:21:36,240 --> 01:21:39,260
Entonces mi propuesta, vuelvo a la...

885
01:21:39,670 --> 01:21:40,840
No, a ver, ¿dónde está?

886
01:21:41,620 --> 01:21:43,360
¿Dónde está? ¿Dónde está? Acá, sí.

887
01:21:44,280 --> 01:21:52,340
dejo de compartir pantalla y les propongo hacer un intervalo de 10 minutos

888
01:21:52,840 --> 01:21:54,360
les parece que volvamos y 40

889
01:21:58,620 --> 01:22:02,780
y quién yo estoy con los auriculares así que si me preguntan por responder

890
01:22:02,860 --> 01:22:05,820
preguntas consultas vamos a ir agandando sobre esto

891
01:22:08,920 --> 01:22:11,520
pero hacemos volvamos y 40

892
01:22:11,520 --> 01:22:14,820
A mí no me quedo bien claro lo que significa el autoestado en sí.

893
01:22:15,260 --> 01:22:21,220
Entendí lo que es el autovalor, pero bueno, no sé si soy yo que no entiendo el auto.

894
01:22:23,140 --> 01:22:28,080
No, bueno, por ahí porque todavía lo tenés muy encaliente.

895
01:22:28,400 --> 01:22:33,420
Después yo voy a actualizar la idea positiva y pongo las formulitas en la idea positiva.

896
01:22:34,640 --> 01:22:36,720
Pero la idea es esta, pero ¿a qué vuelvo a compartir pantalla?

897
01:22:46,400 --> 01:22:50,040
Mi pregunta más contraria es ¿En qué se relaciona el autoestado con el autovalor y el autovalor?

898
01:22:51,800 --> 01:22:58,700
Ah, bueno, no, se relacionan así, definición, auto vector y auto valor.

899
01:22:59,960 --> 01:23:09,360
B es auto vector, auto valor lambda, si, de la, siempre de la matriz A, no, que en este caso represento uno observable,

900
01:23:09,980 --> 01:23:15,000
si A por B es lambda por B, ok, esta es la definición, por definición es así.

901
01:23:18,200 --> 01:23:26,100
Entonces suponete que vos efectivamente calculas, fijas un lambda, podría ser en los casos que

902
01:23:26,200 --> 01:23:32,400
vimos, lambda era uno y menos uno, pero puede haber casos más generales donde tengan otros valores.

903
01:23:37,920 --> 01:23:43,140
¿Me entendés? Entonces fija uno, bueno, para ese, ahora vos puedes ir y calcular un

904
01:23:43,140 --> 01:23:52,060
auto vector, entonces fijemos las cosas, no? sigma x con menos, era -1 por menos, ¿tás

905
01:23:52,100 --> 01:23:55,060
acuerdo? este lo calculamos explícitamente.

906
01:24:02,140 --> 01:24:09,040
Entonces, menos es un autovector de autovalor -1 del observable sigma x.

907
01:24:14,260 --> 01:24:16,120
Bien. -Claro, ahora sí, gracias.

908
01:24:16,760 --> 01:24:23,100
Bien, pero además es autoestado, ¿entendés? ¿Por qué? Porque menos es estado.

909
01:24:25,520 --> 01:24:33,620
Es decir, no es que podría representar a un estado cuántico si vos prepararas a tu sistema en ese estado, entiendes?

910
01:24:35,580 --> 01:24:37,180
Entiendo, sí, sí, sí. Gracias.

911
01:24:37,520 --> 01:24:50,100
Y la idea es esa, que vos al Qubit lo vas a poder preparar en este estado, en realidad si la computadora es universal lo vas a poder preparar en todos los estados que quieras, pero en particular lo puedes preparar en este estado.

912
01:24:51,780 --> 01:24:53,940
Entonces, ¿qué pasaría?

913
01:24:55,320 --> 01:25:04,200
y vos preparas a la computadora cuántica en menos y me dice, bueno te daría el resultado

914
01:25:07,199 --> 01:25:16,720
1 que representa el autovalor -1 y si la preparas en, perdón y me dice en X, te las arreglas para

915
01:25:16,780 --> 01:25:20,760
medir en la dirección X, yo después te voy a enseñar a medir en la computadora cuántica en la

916
01:25:20,760 --> 01:25:30,660
dirección x, me se dice, por ahora no es evidente, pero se puede, pues hay que hacer una triquineuela.

917
01:25:32,390 --> 01:25:39,740
Y si la preparas más y me dicen x, vas a obtener el valor 0 que representa el valor 1,

918
01:25:40,020 --> 01:25:48,280
¿entendés? Es decir, cuando lo ves con spin, puede tomar -1 y 1, y cuando lo ves en términos de

919
01:25:48,280 --> 01:25:53,780
computadora pueden tomar 0 y 1. Es confuso pero en el fondo si lo pensás es una voludez.

920
01:25:54,120 --> 01:25:56,280
Es simplemente una convención.

921
01:26:00,260 --> 01:26:01,420
Respondí tu pregunta.

922
01:26:05,719 --> 01:26:13,239
Va a quedar mi idea. Va quedando, sí. Igual ahora vamos a ver circuitos entonces que va a quedar

923
01:26:13,240 --> 01:26:21,320
un poco más claro, es decir, en algún momento te vas a olvidar un poco de esto y vas a sacar más claro.

924
01:26:27,500 --> 01:26:30,440
Bueno, dejo ahí por si me siguen haciendo preguntas, sigo contestando.

925
01:26:58,520 --> 01:26:59,920
ᴗ �

926
01:27:07,000 --> 01:27:09,800
Yn ymw

927
01:27:37,000 --> 01:27:39,800
Yn ymw

928
01:28:07,000 --> 01:28:09,800
Yn ymw

929
01:28:37,880 --> 01:28:39,800
Yn ymw

930
01:29:07,000 --> 01:29:09,800
Yn ymw

931
01:29:37,000 --> 01:29:39,800
Yn ymw

932
01:30:23,860 --> 01:30:25,260
[Música]

933
01:30:37,000 --> 01:30:43,880
una consulta. ¿Podría pasar en la pizarra que estaba haciendo recién?

934
01:30:55,980 --> 01:30:56,280
¿Está?

935
01:30:58,520 --> 01:31:01,980
Sí, no sé si hay alguna manera de compartirla o algo.

936
01:31:03,300 --> 01:31:04,040
No se ve?

937
01:31:05,020 --> 01:31:10,720
Sí, no digo compartirla porque lo quieres escribir y no llegas a escribir una parte.

938
01:31:12,460 --> 01:31:14,260
ah, te lo digo de vuelta, ¿qué quieres escribir?

939
01:31:16,920 --> 01:31:21,260
no, no, ya desde el principio...

940
01:31:21,260 --> 01:31:26,720
ah, ya te entendí, ya te entendí, si, creo que se puede...

941
01:31:27,300 --> 01:31:28,520
si, de vuelta me la captura la pantalla

942
01:31:29,980 --> 01:31:33,480
si, arriba aparece un botón de jergo, pero no sé qué hará eso

943
01:31:34,420 --> 01:31:37,220
si, que le apretamos si quieres, a ver qué pasa

944
01:31:37,220 --> 01:31:40,980
"copy link" ah si, listo te lo meto por acá

945
01:31:43,300 --> 01:31:45,100
igual después queda el video ¿no? que se yo

946
01:31:46,260 --> 01:31:47,080
en principio

947
01:31:48,180 --> 01:31:51,540
si pero cuando uno lo escribe algo mas que eso

948
01:31:53,640 --> 01:31:54,120
exacto

949
01:31:55,640 --> 01:31:56,560
esperad porque esto...

950
01:32:01,360 --> 01:32:03,140
fíjate ahí si podés ingresar a la...

951
01:32:03,940 --> 01:32:06,220
seguro que te la podés bajar y listo

952
01:32:10,300 --> 01:32:15,560
pasa que todas estas viste pizarras al final son una mierda pues está todo lleno de

953
01:32:16,120 --> 01:32:18,100
van por ahí alguien las a usar bien y

954
01:32:24,120 --> 01:32:27,960
está como yo veo todo muy lleno de que tenés que logrear y

955
01:32:31,560 --> 01:32:35,440
estaría bueno tener alguna herramienta

956
01:32:35,760 --> 01:32:42,440
construida dentro de mi dispositivo y que no sean LAN, no lo sé, tiene sus pro y sus contras.

957
01:32:43,740 --> 01:32:48,820
Comente igual que estamos trabajando en hacer unos resúmenes de las clases,

958
01:32:51,460 --> 01:32:54,380
que esperamos en breve compartir, ok?

959
01:32:55,680 --> 01:32:59,140
cosa que bueno, hacer un complemento para poder estudiar.

960
01:33:01,740 --> 01:33:03,160
¿pudiste bajar la pizarra?

961
01:33:04,560 --> 01:33:08,180
Sí, sí, ahí estaba viendo si la podía exportar en PDF o en imagen.

962
01:33:09,220 --> 01:33:13,900
Claro. Sí, lo que pasa es que igual la pizarra es como muy desprolija, ¿no?

963
01:33:14,100 --> 01:33:17,100
Porque esa es la gracia que uno escribe, borra, se equivoca.

964
01:33:17,360 --> 01:33:19,240
Esa es como la gracia de usar la pizarra.

965
01:33:20,840 --> 01:33:25,180
Por ahí, bueno, yo ya te decía, voy a tratar de completar un poco las diapositivas

966
01:33:25,230 --> 01:33:30,540
con las preguntas que me hicieron, así después les es más fácil ordenarse las ideas.

967
01:33:35,760 --> 01:33:37,060
Bueno, bueno, bueno.

968
01:33:44,020 --> 01:33:46,600
Bueno, voy a seguir, ¿ok?

969
01:33:47,500 --> 01:33:49,520
Sigo con las, con las de positivos.

970
01:33:50,060 --> 01:33:54,900
Igual, no se preocupen si no entendieron porque esto lo vamos a volver a ver más adelante.

971
01:33:55,060 --> 01:33:58,700
pero este es como una primera aproximación al tópico

972
01:34:06,500 --> 01:34:12,480
bien sigo ahora vamos a ver el concepto del producto escalar que es la la

973
01:34:12,560 --> 01:34:16,660
anterior cosa matemática básica crucial del curso

974
01:34:18,440 --> 01:34:23,780
¿Qué es el producto escalar? Bueno, está vinculado a el ángulo entre vectores.

975
01:34:25,210 --> 01:34:26,840
Si ustedes tienen...

976
01:34:30,400 --> 01:34:31,000
Verán qué...

977
01:34:31,480 --> 01:34:31,640
Ahora.

978
01:34:32,880 --> 01:34:33,920
Puedes escribir en la pantalla.

979
01:34:36,240 --> 01:34:41,560
Lo que termina pasando es que si ustedes tienen un espacio vectorial tipo R2 y tienen un vector V1

980
01:34:42,770 --> 01:34:46,520
y otro vector V2, va a haber un ángulo entre estos vectores.

981
01:34:47,020 --> 01:34:49,420
uno se podría preguntar cómo calcula o será ángulo.

982
01:34:50,980 --> 01:34:52,460
Es una pregunta importante.

983
01:34:55,520 --> 01:34:58,120
Y vinculado a eso está la noción de producto escalar.

984
01:34:58,380 --> 01:35:02,240
Supongue que tienen un vector phi y un vector phi.

985
01:35:02,980 --> 01:35:04,240
Cada uno tiene sus coordenadas.

986
01:35:04,640 --> 01:35:09,060
Las de alfa van a ser las de psi y las betas van a ser las de phi.

987
01:35:10,340 --> 01:35:11,960
El producto escalar se define así.

988
01:35:16,060 --> 01:35:17,440
Tiene que hacer...

989
01:35:18,080 --> 01:35:21,160
si, "Raspuesto conjugado", decir...

990
01:35:21,740 --> 01:35:23,040
ahora voy a explicar esto...

991
01:35:23,040 --> 01:35:23,380
el "BRA"

992
01:35:24,760 --> 01:35:26,740
producto matricial contra B1B2

993
01:35:27,680 --> 01:35:30,420
y el producto escalar lo vamos a simbolizar así

994
01:35:32,080 --> 01:35:33,400
y se calcula de esta manera

995
01:35:35,380 --> 01:35:38,020
Tiene que hacer "alpha1" conjugado por beta1

996
01:35:38,520 --> 01:35:41,300
más "alpha2" conjugado por betados, ¿tá bien?

997
01:35:42,960 --> 01:35:45,060
Esto está en el libro de Nielsen y Chuang

998
01:35:45,060 --> 01:36:00,040
es muy importante que lo aprendan y que lo lean también de ahí. Bien, y es alfa 1 alfa 2. ¿Qué es esto de acá?

999
01:36:01,440 --> 01:36:04,240
Feren que voy a notar la pantalla.

1000
01:36:07,800 --> 01:36:16,440
Esto de acá es, si lo ponen al vector columna como está acá arriba es sí, esto es un

1001
01:36:16,540 --> 01:36:18,620
ket, en cuántica se conoce como ket.

1002
01:36:19,060 --> 01:36:25,480
Y si lo ponen así, transpuesto conjugado, fíjense que lo que hice acá es a esto, lo

1003
01:36:25,480 --> 01:36:40,520
pusimos horizontal y después lo conjugamos, esto se conoce como bra, fíjense que tengo

1004
01:36:40,600 --> 01:36:52,200
el ket, esto es el ket y si lo pongo así es el bra, entonces esto es el vector, el ket

1005
01:36:52,200 --> 01:36:59,120
es el vector y el bra es una funcional lineal operando en el espacio de hilo. No vamos a

1006
01:36:59,580 --> 01:37:07,580
entrar en detalle matemático, pero lo importante de la anusación bracket es el bracket. Si

1007
01:37:07,620 --> 01:37:17,760
yo vací que son brackets, es la palabra en inglés bracket, ¿no? Entonces, si esto es

1008
01:37:17,760 --> 01:37:27,540
el ket y esto es el bra cuando braqueteo, hago si, si, si, si contra si, entonces acá

1009
01:37:27,620 --> 01:37:33,700
lo que hice fue el braqueteo, en física decimos braqueteamos, paraquetear braqueteo, hacemos

1010
01:37:33,800 --> 01:37:45,560
el producto braqueteo entre si, acá está bra y acá ponemos si como ket, ok, entonces

1011
01:37:45,560 --> 01:37:55,920
el producto escalares es el bracket. Esta es la notación de bracket de Dirac, se llama

1012
01:37:56,000 --> 01:38:02,920
notación de Dirac y es la notación que van a encontrar en el 99,9% de los textos de teoría

1013
01:38:02,920 --> 01:38:08,860
de la información cuántica, cuántica, computación cuántica, ¿por qué usamos esta notación?

1014
01:38:09,280 --> 01:38:14,620
por ahí para un matemático puede resultar un tanto demencial, bueno, porque simplifica las cuentas.

1015
01:38:15,470 --> 01:38:21,720
Si uno aprende a manipular estos simbolitos de Braeiket, puede hacer las cuentas más rápido,

1016
01:38:21,950 --> 01:38:28,580
sin pensar mucho en qué significa matemáticamente lo que uno está haciendo, ok? Es como una cuestión

1017
01:38:35,780 --> 01:38:40,980
con una cuestión práctica. Voy a seguir con esto, voy a seguir, pues es importante.

1018
01:38:44,260 --> 01:38:49,380
Ypsi es alfa 1, alfa 2, este es el ket,

1019
01:38:50,900 --> 01:38:57,420
entonces el bra significa hacer esto transpuesto con jugado.

1020
01:38:57,640 --> 01:39:01,580
Transponer significa que lo que es columna pasa a ser fila

1021
01:39:02,100 --> 01:39:08,900
y después de conjugar cada uno de los componentes. Recuerden que los componentes del vector son números complejos

1022
01:39:09,230 --> 01:39:11,380
y como son números complejos, los puedo conjugar.

1023
01:39:12,220 --> 01:39:19,100
Que es ellos, si alfa1 es a + b por i, alfa1 conjugado es a - b por i, ¿ok?

1024
01:39:19,880 --> 01:39:20,800
Eso se calcula así.

1025
01:39:22,620 --> 01:39:24,460
Bien, entonces, sí.

1026
01:39:25,100 --> 01:39:27,480
¿Quedó al revés el bra, perdón? Puede ser.

1027
01:39:29,540 --> 01:39:34,520
Sí, me puse este raquet y tengo que poner bra.

1028
01:39:37,960 --> 01:39:40,200
¿Eso mismo no es eso? ¿La daga?

1029
01:39:42,020 --> 01:39:51,900
Sí, lo hace la daga. Claro. Es que es la daga de esta matriz. La daga vale para cualquier matriz, ¿entendés? Por ejemplo, así.

1030
01:39:53,400 --> 01:39:59,660
y lo que es la matriz A=123456

1031
01:40:00,500 --> 01:40:04,720
ay que mala letra, perdón, ya que lo escribo bien en un lado

1032
01:40:05,420 --> 01:40:10,940
vamos a la pizarra esta, así lo hago un poco más claro

1033
01:40:14,160 --> 01:40:19,380
suponente que te hago A=123456

1034
01:40:19,380 --> 01:40:26,400
esta no es cuadrada porque tiene esta pertenece a reales a la 3 por 2

1035
01:40:27,060 --> 01:40:30,120
3 filas, 2 columnas, ¿tabian?

1036
01:40:31,000 --> 01:40:31,100
sí

1037
01:40:32,070 --> 01:40:39,260
a transpuesta es 1, 2, 3, 4, 5, 6 intercambio filas por columnas

1038
01:40:39,980 --> 01:40:40,320
veamos

1039
01:40:41,760 --> 01:40:47,980
si a tiene las componentes a y j cuando transpongo

1040
01:40:48,300 --> 01:40:51,200
La transpuesta tiene las componentes aj y, ¿entendés?

1041
01:40:52,300 --> 01:40:57,020
Y ahora, si transpongo y conjugó, conjugó todos los componentes.

1042
01:40:57,440 --> 01:41:00,920
Acá conjugar da lo mismo porque son reales las entradas de la matriz.

1043
01:41:03,580 --> 01:41:06,600
Pero si hubiera puesto números complejos, los tenía que conjugar, ¿entendés?

1044
01:41:08,020 --> 01:41:15,540
Entonces, si yo tengo un "psi" que es alfa 1, alfa n,

1045
01:41:17,040 --> 01:41:18,560
Este es el "ketz".

1046
01:41:20,300 --> 01:41:27,400
El "bra" va a ser el "si" transpuesto con jugado, alfa 1 con jugado, alfa n con jugado. ¿Está bien?

1047
01:41:30,880 --> 01:41:39,840
Bueno, esto de los "braketz" es crucial. Es crucial en física, por ahí en matemática no lo necesitarían, en realidad no lo necesitan.

1048
01:41:40,980 --> 01:41:47,060
pero en toda la jerga de computación cuántica que usamos los físicos es crucial para entender

1049
01:41:47,120 --> 01:41:48,780
todo lo que hacemos, para leer los libros.

1050
01:41:49,980 --> 01:41:55,620
Bien, así definen el producto escalar para qubits.

1051
01:41:57,780 --> 01:42:05,260
Ahora resulta ser que para vectores reales si toman, por ejemplo, R2, o lo van a pisar

1052
01:42:05,260 --> 01:42:17,620
de la rana. Si toman R2 y tienen 2 vectores, ahora reales, no tomemos R2, y si tienen B

1053
01:42:17,930 --> 01:42:26,740
y W, también B y W van a tener 2 componentes reales y pueden hacer WB contra B. Bueno resulta

1054
01:42:26,760 --> 01:42:33,140
hacer que el producto escalar va a ser un número real y es la norma de W por la

1055
01:42:33,200 --> 01:42:40,980
norma de B por el coseno del ángulo que lo separa. Esto se puede probar, se pueden

1056
01:42:41,100 --> 01:42:42,480
hacer la cuenta y probarlo.

1057
01:42:46,740 --> 01:42:51,180
Entonces el producto escalar que se calcula con esta misma fórmula

1058
01:42:51,180 --> 01:43:03,860
escriben a b y a w con esta misma, pero ahora donde a 1, a 1 y a 2, son números reales

1059
01:43:03,860 --> 01:43:15,520
si tienen b, pa, si se hacen, perdón, se hacen, phi contra psi, esto es lo mismo que la norma

1060
01:43:15,520 --> 01:43:23,520
de phi por la norma de psi por el coseno del ángulo que lo separa, si

1061
01:43:23,560 --> 01:43:28,760
fueran vectores de R2 y si son vectores complejos, es decir, este y este están en

1062
01:43:28,940 --> 01:43:39,440
C2. Esta fórmula, el sí, del módulo del producto escalar, se toma como la

1063
01:43:39,500 --> 01:43:41,120
definición del coseno del ángulo,

1064
01:43:44,239 --> 01:43:44,760
(música)

1065
01:43:49,200 --> 01:43:50,480
¿Eh? ¿Ché? Cuidado.

1066
01:43:51,630 --> 01:43:51,820
Bien.

1067
01:43:54,000 --> 01:43:54,520
Eh...

1068
01:43:55,780 --> 01:43:56,300
(música)

1069
01:44:00,680 --> 01:44:04,180
Ahora me... No me acuerdo si tengo que ponerlo al cuadrón o no, pero no importa.

1070
01:44:04,630 --> 01:44:09,360
Lo importante es que el módulo del producto escalar

1071
01:44:10,210 --> 01:44:13,020
va a ser proporcional al coceno del ángulo, ¿eh?

1072
01:44:13,130 --> 01:44:13,260
(más risas)

1073
01:44:14,520 --> 01:44:17,020
va a estar vinculado al ángulo entre los dos vectores.

1074
01:44:18,680 --> 01:44:21,320
Después lo escribo bien en las diapositivas, lo del ángulo.

1075
01:44:22,740 --> 01:44:25,640
Pero lo que van a tener que usar en este curso es esto,

1076
01:44:26,360 --> 01:44:29,060
esto de acá, esta fórmula de acá.

1077
01:44:29,660 --> 01:44:32,480
Así que recuerden, así se cancube el producto escala.

1078
01:44:32,940 --> 01:44:35,800
Está también el libro de An-se-chuan, todos los libros.

1079
01:44:36,250 --> 01:44:39,860
Y si tienen un espacio de dimensión N, es decir,

1080
01:44:40,260 --> 01:44:43,000
Acá está en el diapositiva anterior, estábamos en C2.

1081
01:44:43,940 --> 01:44:46,720
Suponga que están en CN, en un espacio de dimensión N.

1082
01:44:47,520 --> 01:44:50,580
Entonces cada vector tiene N entre adicas complejas.

1083
01:44:52,050 --> 01:44:58,220
Bien, entonces acá también tiene que hacer bra contra ket.

1084
01:44:59,270 --> 01:45:00,260
Y se calcula así.

1085
01:45:00,940 --> 01:45:04,900
Alpha 1 con jugado por beta 1, más alpha 2 con jugado por beta 2.

1086
01:45:06,360 --> 01:45:13,680
acá, acá, este no va, acá, este después le borro, con el espacio de la posibilidad,

1087
01:45:13,880 --> 01:45:25,540
este puse de más, más alfane por beta n. Bien, y esto es lo mismo y acá de vuelta,

1088
01:45:25,780 --> 01:45:33,320
este no va. Esta formulita está también en el Nielsen y Chuang, este no. Suma de alfa

1089
01:45:33,320 --> 01:45:37,900
hay conjugado por Betai, esta es la forma compacta de escribir y definir el producto escalar.

1090
01:45:38,070 --> 01:45:45,200
¿Está bien? Hay una pregunta. Es una fórmula. Después esto lo pueden hacer en Python. Ya

1091
01:45:45,200 --> 01:45:54,180
la semana que viene todas estas cosas la vamos a ver en Python. ¿Ok? Bien. ¿Y por qué todo

1092
01:45:54,240 --> 01:45:58,060
Esto es importante, bien, porque la probabilidad de transición,

1093
01:45:59,980 --> 01:46:01,940
piensan en esto, supongo que

1094
01:46:05,800 --> 01:46:08,120
tienen, ¿qué es eso? un átomo o lo que sea

1095
01:46:09,200 --> 01:46:13,160
y tienen el estado si y tiene el estado si.

1096
01:46:14,640 --> 01:46:20,420
¿Cuál es la probabilidad sísica de que si el sistema está en el estado si,

1097
01:46:21,200 --> 01:46:23,480
si ustedes lo observen en el estado si?

1098
01:46:24,240 --> 01:46:30,640
o que salte. Bueno, esta probabilidad de transición está dado por el módulo del producto escalar al cuadrado.

1099
01:46:31,320 --> 01:46:34,900
Esto es lo que les importa usted, cíficamente. Esto es lo que tienen que recortar.

1100
01:46:35,420 --> 01:46:36,560
Se llama regla de Borm.

1101
01:46:38,440 --> 01:46:42,620
Es la probabilidad de transición de "psi" a "fi".

1102
01:46:43,240 --> 01:46:46,560
Ok? Bueno, acá estoy usando la letrita...

1103
01:46:47,120 --> 01:46:48,240
Péren, "fi".

1104
01:46:52,420 --> 01:46:56,700
Péren que lo escribo. Probabilidad de transición de "si" a "fi".

1105
01:46:58,180 --> 01:47:01,220
Fíjense que la probabilidad, por cómo está definida la fórmula,

1106
01:47:02,140 --> 01:47:06,120
probabilidad de "si" a "fi" es lo mismo que la probabilidad de "si" a "fi".

1107
01:47:07,300 --> 01:47:10,900
Da lo mismo. Podría no ser así, pero en física cuántica es así.

1108
01:47:11,200 --> 01:47:13,680
Uno podría inventar una teoría que no es la cuántica,

1109
01:47:13,680 --> 01:47:19,660
en la cual la probabilidad de transición no es simétrica, pero justo en cuántica es

1110
01:47:19,820 --> 01:47:26,180
simétrica. ¿Por qué es esto? Bueno, porque el módulo de "c" contra "c" al cuadrado

1111
01:47:26,480 --> 01:47:31,300
es igual al módulo de "c" contra "c" al cuadrado. Esto lo pueden probar, ¿está bien?

1112
01:47:32,020 --> 01:47:42,320
Entonces, esta magnitud, la magnitud "c" contra "c" se llama amplitud de probabilidad,

1113
01:47:43,360 --> 01:47:49,020
se llama amplitud de probabilidad

1114
01:47:51,920 --> 01:47:54,600
ok, esto es la amplitud de probabilidad

1115
01:47:55,160 --> 01:47:58,240
y esto es la...

1116
01:47:59,060 --> 01:48:01,580
el módulo al cuadrado es la probabilidad ok

1117
01:48:03,320 --> 01:48:07,520
es decir, si la amplitud de probabilidad es el número complejo z

1118
01:48:08,660 --> 01:48:12,360
entonces la probabilidad es el módulo al cuadrado de z

1119
01:48:12,420 --> 01:48:17,860
Siempre esta amplitud de probabilidad es un número, en el caso más general puede ser un número complejo.

1120
01:48:17,930 --> 01:48:24,260
Entonces, en cuántica las probabilidades se calculan así, uno tiene un estado y tiene otro.

1121
01:48:25,430 --> 01:48:31,620
Y entonces va a ver cuál es la amplitud de probabilidad de transicionar de un estado a otro.

1122
01:48:31,780 --> 01:48:36,980
Eso lo van a ver en los libros. La amplitud de probabilidad de observar tal cosa es esto.

1123
01:48:36,980 --> 01:48:42,440
Bueno, eso todavía no es la probabilidad. La amplitud de probabilidad va a venir dada por este brackets,

1124
01:48:42,940 --> 01:48:45,820
por hacer el producto escalar entre los dos estados.

1125
01:48:47,020 --> 01:48:50,640
Y la probabilidad va a ser el módulo al cuadrado de la amplitud de probabilidad, ¿ok?

1126
01:48:52,040 --> 01:48:56,380
Esto lo borro todo, esto es bueno. Probabilidad de transición es esto.

1127
01:48:57,080 --> 01:49:00,980
Y el valor medio de un observable va a venir dado por...

1128
01:49:01,340 --> 01:49:06,900
es decir, perdón, valor medio de un observable, si el sistema está preparado en el estado

1129
01:49:07,060 --> 01:49:13,120
"psi", el valor medio es esta formulita acá, "psi" por "a" por "psi", que sería hacer

1130
01:49:13,220 --> 01:49:24,300
el bracket entre "psi" y "a" por "psi". Con esta formulita calculan el valor medio,

1131
01:49:24,460 --> 01:49:28,460
por ejemplo, de la energía, el valor medio del spin, el valor medio de cualquier otra

1132
01:49:28,460 --> 01:49:35,300
magnitud que quieren estudiar. Entonces, estas son las dos si quieren cuentas clave del curso,

1133
01:49:35,960 --> 01:49:41,640
o de cualquier curso de física cuántica. Una es cómo calcular la prioridad de transición entre

1134
01:49:41,640 --> 01:49:47,700
un estado y otro. Y la otra es cómo calcular el valor medio de un observable. Esto es todo lo que

1135
01:49:47,900 --> 01:49:52,360
necesitan para describir la física de un problema, junto con, por supuesto, su evolución dinámica.

1136
01:49:52,360 --> 01:49:57,000
cómo va a ser especificar, cómo va a ser la evolución dinámica. Bueno, alguna pregunta?

1137
01:50:02,480 --> 01:50:09,340
Bien, entonces sigo. Y ahora vamos a empezar a ver ya el concepto de entrelazamiento.

1138
01:50:09,820 --> 01:50:16,680
Y para ver el concepto de entrelazamiento tenemos que ver el último concepto matemático clave,

1139
01:50:16,680 --> 01:50:23,520
que es el producto tensorial. Si tengo un estado "psi" y un estado "psi" prima, los escribo en

1140
01:50:23,540 --> 01:50:30,340
componentes alfa, beta y alfa, prima y beta prima, el producto tensorial entre estos se calcula con

1141
01:50:30,420 --> 01:50:37,780
esta fórmula. Esto está así también en el libro Daniel Sanchon, tiene que hacer esta formulita.

1142
01:50:38,660 --> 01:50:42,440
La semana que viene lo hacemos directamente con Python, todo esto lo puede hacer con Python,

1143
01:50:42,520 --> 01:50:46,160
todas estas herramientas están en la librería "Numpi"

1144
01:50:47,640 --> 01:50:49,380
después les voy a enseñar cómo calcularlo

1145
01:50:50,820 --> 01:50:52,080
y tienen que aplicar esta fórmula

1146
01:50:52,440 --> 01:50:56,700
¿Cómo es? Bueno, el "psi" tiene componentes "alpha" y "beta"

1147
01:50:56,790 --> 01:50:58,500
y el "psi" prima, "alpha" veta prima

1148
01:50:58,780 --> 01:51:01,900
entonces en la primera componente del resultado del producto

1149
01:51:02,660 --> 01:51:04,720
hacen el primero de "psi"

1150
01:51:05,970 --> 01:51:07,700
contra el primero de "psi" prima

1151
01:51:08,980 --> 01:51:12,500
después hacen el primero de "psi" contra el segundo de "psi" prima

1152
01:51:12,500 --> 01:51:16,600
eso les da las dos primeras componentes del producto tensorial y después hacen lo

1153
01:51:16,620 --> 01:51:21,600
mismo con la segunda, beta por el fa prima y beta por beta prima, así nomás.

1154
01:51:22,780 --> 01:51:29,200
Ok, no hay ningún misterio, es una cuenta. Ahora esto es importante porque

1155
01:51:29,940 --> 01:51:33,500
permite describir a dos sistemas cuánticos, porque supongan que tienen un

1156
01:51:33,660 --> 01:51:36,900
átomo que está en el estado psi

1157
01:51:37,960 --> 01:51:41,400
y tienen a otro átomo que está en el estado "ciprima".

1158
01:51:42,900 --> 01:51:45,020
Bien, ¿cuál es el estado de los dos átomos juntos?

1159
01:51:45,180 --> 01:51:47,200
Bueno, tienen que hacer el producto tensorial.

1160
01:51:47,760 --> 01:51:51,360
Entonces, este vector de acá representa al estado cuántico

1161
01:51:52,600 --> 01:51:53,980
del sistema conjunto.

1162
01:51:55,340 --> 01:51:58,000
¿Te entiendes? Una cosa es escribir a un sistema cuántico,

1163
01:51:59,580 --> 01:52:02,560
a un qubit, pero la computadora cuántica va a tener n qubits,

1164
01:52:02,860 --> 01:52:04,720
va a tener n sistemas cuánticos,

1165
01:52:05,540 --> 01:52:12,860
donde N, ojalá sea muy grande en el futuro cercano.

1166
01:52:12,980 --> 01:52:16,800
Por ahora tienen decenas de qubits, o ya tienen una centena,

1167
01:52:17,960 --> 01:52:19,040
depende del dispositivo.

1168
01:52:19,980 --> 01:52:23,800
Pero para representar al estado de múltiples qubits,

1169
01:52:24,400 --> 01:52:26,780
tienen que hacer esto que se conoce como producto

1170
01:52:26,860 --> 01:52:27,320
tensorial.

1171
01:52:27,520 --> 01:52:29,820
Ojo, una cosa es el producto escalar.

1172
01:52:30,920 --> 01:52:34,160
Cuando hacen sí contra sí prima.

1173
01:52:35,260 --> 01:52:39,040
Esto es un número complejo y dijimos que era la amplitud de probabilidad.

1174
01:52:39,260 --> 01:52:43,540
Ahora el producto tensorial da un vector.

1175
01:52:46,620 --> 01:52:48,320
Esto pertenece a c4.

1176
01:52:52,440 --> 01:52:54,440
Ven que acá, esta ya la tiro.

1177
01:52:56,659 --> 01:53:00,740
Fíjense, este de acá está en c2.

1178
01:53:01,840 --> 01:53:03,640
El alfa primero, beta primero está en c2.

1179
01:53:03,860 --> 01:53:09,020
cuando hay el producto tensorial, tengo ahora cuatro números complejos, una tira de 4, entonces

1180
01:53:13,300 --> 01:53:15,800
este está en C2, este está en C2

1181
01:53:17,380 --> 01:53:22,740
y esta está en C a la 2 por 2, que es igual a C4

1182
01:53:24,820 --> 01:53:27,260
en realidad no se lo... con la notación que estamos usando acá

1183
01:53:28,880 --> 01:53:31,900
es que es C4 de 1, es un chorizo de 4, ok?

1184
01:53:33,880 --> 01:53:41,460
Bueno, es una fórmula en el libro de Nielsen y Chong tienen varios ejercicios, haganlos,

1185
01:53:41,880 --> 01:53:50,280
haganlos de producto escalar, hagan todo, leanlo línea por línea, es muy importante que además

1186
01:53:50,280 --> 01:53:52,460
de seguir las clases vayan leyendo esto.

1187
01:53:56,100 --> 01:54:00,160
Y bueno, y es muy importante que repitan en sus casas estas cuentas de acá, ¿ven?

1188
01:54:01,300 --> 01:54:03,140
vamos a usar esta notación todo el tiempo.

1189
01:54:04,280 --> 01:54:08,720
Ejemplo, vamos a hacer 0 producto tensoridad 0.

1190
01:54:09,080 --> 01:54:10,160
Esto es para un qubit, ¿no?

1191
01:54:11,340 --> 01:54:14,920
Entonces, tengo el primer qubit en 0 y ahora tengo dos qubits,

1192
01:54:16,550 --> 01:54:21,880
que es yo, un atomico que está en 0 y otro atomito que está en 0.

1193
01:54:23,260 --> 01:54:25,600
Entonces, ¿cómo es el estado del sistema conjunto?

1194
01:54:25,900 --> 01:54:26,960
0 tensor 0.

1195
01:54:28,100 --> 01:54:34,240
esto, acá estoy poniendo explícitamente el producto, pero a veces me lo voy a sacar de

1196
01:54:34,300 --> 01:54:40,140
encima al producto y voy a poner directamente 0 con 0. Esto 0, 0 quiere decir que el primer

1197
01:54:40,300 --> 01:54:46,480
quíbito está en 0 y el segundo quíbito está en 0. Bien, vamos a la cuenta. El 0 era

1198
01:54:46,480 --> 01:54:52,340
el vector 1, 0. Para cada uno de los dos y cuando aplico la formulita de la vida positiva

1199
01:54:52,340 --> 01:55:00,040
anterior tengo que hacer 1 por 1, 1, 1 por 0, 0. 0 por 1, 0, es este 0 de acá y 0 por

1200
01:55:00,220 --> 01:55:02,000
0, 0, es este 0 de acá, está bien?

1201
01:55:07,820 --> 01:55:19,780
También podría tener 0 por 1, ¿no? El primer, el, al primer átomo en 0 y al

1202
01:55:19,780 --> 01:55:27,640
segundo átomo en uno. Bien, este va a ser el estado 0-1, entonces tengo que hacer el 1-0

1203
01:55:28,640 --> 01:55:36,560
por el 0-1, entonces hago 1 por 0, 0, le pongo acá, 1 por 1-1, le pongo acá, 0 por 0-0, le pongo acá

1204
01:55:36,680 --> 01:55:39,060
y 0 por 1-0, le pongo acá

1205
01:55:49,780 --> 01:55:50,580
van ustedes esto.

1206
01:55:53,580 --> 01:55:57,620
Ahora con estos 4, con 0, 0, 1, 0, 0, 1, 1, 1, 1,

1207
01:55:57,620 --> 01:56:00,460
me armo lo que se conoce una base para 2 qubits.

1208
01:56:00,980 --> 01:56:03,240
Esta es la base de 2 qubits.

1209
01:56:04,960 --> 01:56:09,200
Acá lo puse explícitamente, el 1, 0, 0, 0, 0, 1, 0, 0, etcétera.

1210
01:56:10,620 --> 01:56:14,180
¿Qué quiere decir que esto es una base para el espacio de 2

1211
01:56:14,240 --> 01:56:14,600
qubits?

1212
01:56:14,960 --> 01:56:17,660
Bueno, quiere decir que cualquier estado de 2 qubits,

1213
01:56:17,820 --> 01:56:23,400
o dos sistémicas cuánticos de los niveles, se escribe como combinación lineal de vectores

1214
01:56:23,400 --> 01:56:28,620
de la base arriba. Quiere decir que cualquier estado de los dos qubits se puede escribir

1215
01:56:28,800 --> 01:56:35,000
como un alfa 1 por 0, 0 más un alfa 2 por 1, 0 más un alfa 3 por 0, 1 y así. Y esto

1216
01:56:35,180 --> 01:56:42,100
me da en la representación de coordenadas un chorizo vertical con cuatro números complejos.

1217
01:56:43,280 --> 01:56:49,800
pertenece a c4 y recuerden que para que ps2 sea un estado cuántico se tiene que

1218
01:56:49,900 --> 01:56:55,140
cumplir la condición de normalización de abajo que la suma de los módulos al

1219
01:56:55,180 --> 01:56:59,160
cuadrado de los componentes tiene que ser igual a 1. Esto es lo mismo que pedir que la

1220
01:56:59,220 --> 01:57:06,240
norma de este vector ps2 sea igual a 1. Recordar que acá cada uno de los alfa y

1221
01:57:06,240 --> 01:57:08,160
es un numerito complejo. ¿Está bien?

1222
01:57:11,640 --> 01:57:12,420
Bueno, alguna pregunta?

1223
01:57:19,620 --> 01:57:25,300
Bien, sigo. Yo tengo una profe. Sí. Para el producto tensorial no hace falta que

1224
01:57:25,400 --> 01:57:30,740
sean del mismo tamaño los vectores, ¿no? No, exacto, no. Ahora, ahora lo vemos,

1225
01:57:30,800 --> 01:57:38,680
porque ves acá voy a hacer el producto tensorial de 3, tengo de 3 qubits.

1226
01:57:42,760 --> 01:57:48,940
Entonces fíjate que ahora voy a tener, esta buena pregunta porque es importante.

1227
01:57:50,390 --> 01:57:58,520
Yo primero voy a tener, tengo que hacer si1 tensor, si2 tensor, si3.

1228
01:57:59,900 --> 01:58:08,960
Pero ustedes van a tener que hacer primero, si 1 tensor si 2, y a ese coso que tiene 4, tiene dimensión 4, le tienen que multiplicar si 3, ¿entendés?

1229
01:58:09,820 --> 01:58:10,040
Sí.

1230
01:58:11,580 --> 01:58:12,820
Pero es la misma, ¿por qué?

1231
01:58:13,870 --> 01:58:14,640
Claro, es asociativo.

1232
01:58:16,000 --> 01:58:27,800
Si 2 tenés un alfa 1, alfa 2, alfa 3, alfa 4, y haces tensor por un beta 1, y un beta 2, seguís la misma lógica, así es, alfa 1, beta 1, lo pones acá.

1233
01:58:28,340 --> 01:58:34,760
alfa2, betado lo pones acá, después lo pones acá, alfa2, betado lo pones acá, alfa3, betado1

1234
01:58:34,760 --> 01:58:37,700
y así y ahora te queda de tamaño 8, ¿entendés?

1235
01:58:39,600 --> 01:58:40,080
Sí, sí.

1236
01:58:41,190 --> 01:58:46,120
Que eso es un poco lo que yo puse acá, ¿ves? Acá te defino los vectores, ¿no?

1237
01:58:48,160 --> 01:58:57,780
Y luego, una forma de verlo a esto es hacer todos contratodos y agrupar, ¿ves? Puse...

1238
01:58:57,780 --> 01:59:02,520
Eso es interesante o útil esta notación de brackets, porque te permita hacer estas

1239
01:59:03,620 --> 01:59:11,900
como estos juegitos de nomenclatura, juegitos, estas manipulaciones de símbolos básicamente,

1240
01:59:12,400 --> 01:59:14,320
sin por ahí entender mucho lo que está pasando dentro.

1241
01:59:15,280 --> 01:59:18,080
Pero lo que hay que hacer, si uno, ten sorpsi dos, ten sorpsi tres.

1242
01:59:19,480 --> 01:59:24,460
Entonces bueno, tengo que hacer todos contra todos, algo este por este, es como si cierras

1243
01:59:24,460 --> 01:59:29,600
distributiva y los va juntando, entonces te queda alpha1, alpha2, alpha3 por 0, 0, 0,

1244
01:59:29,820 --> 01:59:34,880
alpha1, beta2, alpha3, 0, 1, 0, 0, esto también algo como ejercicio en casa, ok?

1245
01:59:36,320 --> 01:59:46,480
Super importante que lo repita, bien. Y así, y así, ya hacen 0, 0, 0, acá, esto sería

1246
01:59:46,700 --> 01:59:54,440
B3, que sería la base del espacio vectorial para 3 qubits. Bueno, les va a quedar haciendo

1247
01:59:54,440 --> 01:59:58,900
de productos tensoriales posibles, les queda esto, esto es una base.

1248
02:00:00,220 --> 02:00:01,060
¿Base de qué espacio?

1249
02:00:06,320 --> 02:00:09,740
Esto es una base del espacio vectorial C8.

1250
02:00:10,620 --> 02:00:12,700
Acá los vectores son

1251
02:00:14,280 --> 02:00:16,500
tiras verticales de largo 8.

1252
02:00:19,960 --> 02:00:30,640
un vector típico de C8 va a ser una cosa así, va a ser alfa 1, alfa 2, hasta alfa 8, va a ser 8 coordenadas complejas

1253
02:00:32,660 --> 02:00:40,440
y esto es una base, queriendo decir que cada vector de C8 se escribe como combinación lineal de estos elementos de la base

1254
02:00:40,440 --> 02:00:43,600
y acá están puestos cada uno de los elementos de la base explícitamente.

1255
02:00:44,300 --> 02:00:52,180
Ejercicio o calcularlos, calcular que 0, 0, 0 es el 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0,

1256
02:01:10,440 --> 02:01:15,240
el 1, 0, producto tensorial el 1, 0, ok?

1257
02:01:17,140 --> 02:01:26,360
y por ejemplo el 0, 1, 0 sería el 1, 0, producto tensorial 0, 1, producto tensorial 1, 0

1258
02:01:27,760 --> 02:01:31,500
bueno, haciendo esto, estas cuentas van a encontrar eso, ¿sí?

1259
02:01:34,520 --> 02:01:46,020
Bien, y esta sería una base, o esta se conoce como la base computacional para el espacio

1260
02:01:46,140 --> 02:01:47,440
vectorial de 3 qubits.

1261
02:01:50,040 --> 02:01:51,540
Bueno, ¿qué pasa si tienen...

1262
02:01:51,540 --> 02:01:55,280
Bueno, y acá me comí una...

1263
02:02:00,980 --> 02:02:05,660
Un corchete ahí, un R-angle en látex.

1264
02:02:06,920 --> 02:02:11,380
Bien, es decir, B3 es una base del espacio.

1265
02:02:12,640 --> 02:02:18,380
Lo cual quiere decir que cualquier vector se escribe como combinación lineal de estos elementos.

1266
02:02:19,840 --> 02:02:29,280
Y cualquier vector, esto va a estar en c a la 8, es una tira, una columna con 8 componentes complejas.

1267
02:02:31,420 --> 02:02:37,280
Para que esto tefine a un estado cuántico, legítimo, se tiene que cumplir la condición de normalización que le escribí acá,

1268
02:02:38,280 --> 02:02:42,080
que es que la suma de los módulos al cuadrado de los coeficientes se evola a 1.

1269
02:02:44,780 --> 02:02:49,340
que en el fondo no es otra cosa más que la condición de normalización de la probabilidad.

1270
02:02:49,480 --> 02:02:59,080
¿Cómo le vamos a ver a lo largo de las distintas clases? Bien. Esto era para tres qubits y bueno,

1271
02:02:59,200 --> 02:03:04,620
si tienen n qubits es lo mismo. Ahora puse sus pustitos subpensivos porque para n qubits

1272
02:03:04,700 --> 02:03:14,080
van a ver n0s y lo importante, y esto tiene que ver con la complejidad de las computadoras

1273
02:03:14,140 --> 02:03:21,400
cuánticas, al menos con la complejidad en términos de memoria, la dimensión del espacio

1274
02:03:21,520 --> 02:03:27,040
vectorial crece como 2 a la n, donde n es el número de qubits, es decir, si tienen 4 qubits

1275
02:03:28,660 --> 02:03:38,320
para n=4 la dimensión va a ser 16, para n=5 la dimensión va a ser 32 y así siguiendo,

1276
02:03:38,520 --> 02:03:44,620
para n=10 va a ser 1024 y así, entonces la dimensión de la base del espacio vectorial

1277
02:03:47,140 --> 02:03:55,740
crece exponencialmente con el número de qubits, si tienen 10 sistemas cuánticos, la dimensión

1278
02:03:55,740 --> 02:04:02,080
del espacio vectorial es 2 a la 10 y la base computacional va a tener 2 a la 10 que es 1024

1279
02:04:02,360 --> 02:04:10,700
elementos. Piensen que esto es un número brutal porque si tengo 100 qubits la dimensión del

1280
02:04:10,760 --> 02:04:16,940
espacio es 2 a la 100 que ya es un número muy grande. Si ustedes tienen que representar un vector

1281
02:04:17,060 --> 02:04:23,420
complejo de dimensión 2 a la 100, bueno, necesito una cantidad de memoria muy grande. ¿Se entiende

1282
02:04:23,420 --> 02:04:33,120
porque ya de entrada si quiero representar un vector de un sistema cuántico muy grande ya de entrada

1283
02:04:33,160 --> 02:04:41,620
tengo un problema de memoria directamente, pues tengo que almacenar un vector complejo de tamaño 2

1284
02:04:42,080 --> 02:04:50,860
a la n donde n es el número de componentes. Entonces esta sería la base computacional de n qubits y

1285
02:04:50,860 --> 02:04:52,980
que tiene 2 a la n elementos

1286
02:04:55,760 --> 02:04:58,880
cualquier vector de este espacio, esto sería

1287
02:05:00,520 --> 02:05:02,880
un vector de acá, perdón

1288
02:05:07,760 --> 02:05:13,200
un vector de acá, por Tnc a c a la 2 a la n, lo he escrito acá abajo

1289
02:05:14,100 --> 02:05:17,860
si los vector es estos están c a la 2 a la n

1290
02:05:17,860 --> 02:05:20,440
de "n" es el número de componentes.

1291
02:05:22,900 --> 02:05:25,720
Entonces esto, graven celo, esta es la base computacional.

1292
02:05:26,140 --> 02:05:26,680
¿Alguna pregunta?

1293
02:05:33,540 --> 02:05:35,860
Bien, si no hay preguntas, veamos.

1294
02:05:37,180 --> 02:05:38,520
Vamos a dar otra definición.

1295
02:05:38,740 --> 02:05:39,960
Ahora sí una definición física.

1296
02:05:40,260 --> 02:05:42,460
Ya terminamos con las definiciones matemáticas,

1297
02:05:42,510 --> 02:05:43,040
por suerte.

1298
02:05:43,580 --> 02:05:45,480
Pero ahora ya vamos a las definiciones físicas.

1299
02:05:46,540 --> 02:05:55,100
vamos a dar la noción de enterazamiento. Si tengo dos qubits, si tengo dos qubits, puedo preparar el estado 0,0,

1300
02:05:55,630 --> 02:06:01,680
es decir, el primero en cero y el segundo en cero. También puedo preparar el 1,1, el primero en uno y el segundo en uno.

1301
02:06:02,870 --> 02:06:07,300
Y utilizando el principio de superposición, puedo armar una combinación lineal de estos dos.

1302
02:06:07,540 --> 02:06:11,000
Entonces puedo armar una superposición equiprobable,

1303
02:06:11,520 --> 02:06:15,080
probabilidad 50%, entre 0 y 0 y 1 y 1.

1304
02:06:15,200 --> 02:06:20,360
Es como una moneda en la cual la mitad de las veces tengo el

1305
02:06:20,380 --> 02:06:23,280
sistema en 0, 0 y la mitad de las veces tengo el sistema

1306
02:06:23,620 --> 02:06:26,120
conjunto, en 0, 1, si ya los 2 quibis juntos.

1307
02:06:27,740 --> 02:06:29,060
Este es un estado entrelazado.

1308
02:06:29,840 --> 02:06:31,020
¿Qué es un estado entrelazado?

1309
02:06:31,160 --> 02:06:34,940
Bueno, un estado que no se puede escribir como un producto

1310
02:06:34,940 --> 02:06:40,480
tensorial para los dos sistemas, de los dos sistemas.

1311
02:06:42,840 --> 02:06:50,940
Porque atención, uno podría pensar ingenuamente que siempre que tenga un Qubit y tenga otro,

1312
02:06:53,780 --> 02:07:00,280
siempre puede tener que el estado de los dos Qubit va a ser un C-tensor, o un C1 o un C2,

1313
02:07:01,260 --> 02:07:07,800
Si uno dice "bueno, si el estado del sistema conjunto es el producto tensorial, bien, entonces

1314
02:07:08,860 --> 02:07:14,280
siempre voy a poder escribir el estado de los dos qubits como un producto tensorial".

1315
02:07:14,280 --> 02:07:16,740
Bueno, no, esto no es así.

1316
02:07:17,570 --> 02:07:23,280
Hay estados que no se escriben como un producto tensorial directo, sino como una combinación

1317
02:07:23,380 --> 02:07:25,620
lineal de producto tensorial, ¿te entiendes?

1318
02:07:26,780 --> 02:07:33,140
es decir, acá hice 0, 0, 1, 1 y después hice una superposición entre esos dos.

1319
02:07:33,230 --> 02:07:37,580
Es como un gato de Schrodinger para estos dos estados.

1320
02:07:39,870 --> 02:07:41,580
Entonces esta es la noción de enterazamiento.

1321
02:07:42,620 --> 02:07:50,200
Un estado cuántico está entrelazado si no es posible escribir a dicho estado como un

1322
02:07:50,220 --> 02:07:54,460
producto tensorial de estados de los componentes.

1323
02:07:57,900 --> 02:08:02,440
¿Cuál es la gracia de los estados entrelazados? Bueno, que tienen propiedades

1324
02:08:03,940 --> 02:08:08,940
que van más allá de las propiedades de los estados clásicos en el sentido de

1325
02:08:08,940 --> 02:08:15,421
que se pueden producir correlaciones que no se pueden modelar

1326
02:08:15,420 --> 02:08:21,400
clasicamente, o que no se pueden emular con sistemas clásicos, esa es la idea de los Estados

1327
02:08:21,500 --> 02:08:32,180
Entrasados. Bien, ya estamos bastante avanzados, voy a seguir con esto, no espero que lo entiendan

1328
02:08:32,180 --> 02:08:37,520
a todo esto ahora, pero ya con esto tiene mucho material para profundizar en la bibliografía,

1329
02:08:38,380 --> 02:08:44,980
que también yo les puse en la página de la materia una entrada del leccionario austral

1330
02:08:46,080 --> 02:08:53,420
que es un artículo de Jeffrey Pope explicando lo que es el entrasamiento cuántico. Eso ya lo

1331
02:08:53,620 --> 02:08:59,240
podrían leer, que es el "Están castellanos" y también tienen para leer por supuesto el libro de

1332
02:08:59,240 --> 02:09:13,760
Daniel Senechor. ¿Haga una pregunta? Bueno, no, ¿cómo vienen? Les estoy matando, esa

1333
02:09:13,880 --> 02:09:21,200
es una locura, todo esto. Y hay que estudiar, hay que sentarse y...

1334
02:09:22,480 --> 02:09:26,880
Hay que estudiar, pero está bueno porque es importante estudiar todo esto porque te

1335
02:09:26,880 --> 02:09:32,100
y obliga a aprender al gelalinial y después encima vas a aprender un poco a implementar

1336
02:09:32,110 --> 02:09:36,800
todo esto en Python, lo cual es una herramienta bastante poderosa, más allá de que después

1337
02:09:36,940 --> 02:09:41,980
hagas cuántica o no, después te puedes servir en la vida, pues estas cosas aparecen cada

1338
02:09:42,100 --> 02:09:47,800
dos por tres en programación, viste, desde resolver sistemas de ecuaciones lineales hasta

1339
02:09:48,180 --> 02:09:54,760
que sé yo, la matriz, insumo producto, no sé, viste, tenés que saber multiplicar matriz

1340
02:09:54,760 --> 02:09:56,020
y hacer operatorias con matrices.

1341
02:09:57,040 --> 02:09:57,160
Bien.

1342
02:09:58,900 --> 02:10:02,040
Y bueno, solo lo repito por completitud, ¿no?

1343
02:10:03,239 --> 02:10:03,880
En...

1344
02:10:06,180 --> 02:10:11,440
La evolución dinámica del sistema venía dada por la multiplicación por una matriz unitaria.

1345
02:10:11,620 --> 02:10:14,860
Y este era el concepto de comporta lógica cuántica.

1346
02:10:18,760 --> 02:10:24,660
y las matrices unitarias cumplían con esta condición de que

1347
02:10:25,959 --> 02:10:29,260
"Ustrafuesta conjugada" es la inversa de la matrices.

1348
02:10:34,960 --> 02:10:38,360
Entonces, vamos a ver o ya vimos que la evolución dinámica,

1349
02:10:38,410 --> 02:10:42,000
si el estado, si empezábamos con "psi"

1350
02:10:43,559 --> 02:10:45,920
cuando transformamos el estado del sistema,

1351
02:10:46,760 --> 02:10:51,420
evolución va a estar matemáticamente representada por la multiplicación

1352
02:10:51,640 --> 02:10:55,980
matricial entre U y el estado Opsi. ¿Qué es una cuenta muy sencilla? Ya lo

1353
02:10:56,100 --> 02:11:01,620
digo. Bien. Y así son las comportas lógicas cuánticas.

1354
02:11:02,260 --> 02:11:06,960
Ok. Así son las comportas lógicas cuánticas. Entonces una comporta famosa es

1355
02:11:06,960 --> 02:11:09,140
Jadamard, este...

1356
02:11:11,680 --> 02:11:13,100
En este dibujo de acá,

1357
02:11:17,280 --> 02:11:18,740
vamos acá, explico ¿no?

1358
02:11:19,300 --> 02:11:21,500
La línea horizontal representa el qubit

1359
02:11:23,300 --> 02:11:26,940
y lo que yo voy poniendo en el medio de las cajitas o cuadraditos

1360
02:11:27,440 --> 02:11:28,860
son las operaciones lógicas.

1361
02:11:29,140 --> 02:11:32,340
Acá apliqué una U, acá apliqué otra U distinta y así.

1362
02:11:34,620 --> 02:11:36,840
Es decir, esto es un circuito cuántico.

1363
02:11:36,940 --> 02:11:39,460
Es un circuito cuántico que tiene un qubit,

1364
02:11:40,260 --> 02:11:50,920
le aplico a este qubit, la matriz Hadamard, que es la comporta lógica Hadamard y después

1365
02:11:50,960 --> 02:11:58,040
el qubit sigue. Entonces, si preparo el qubit en un estado inicial que es 0 y le aplico la

1366
02:11:58,100 --> 02:12:05,941
matriz Hadamard, bueno, ustedes hacen la cuenta de que h por 0 da más. Entonces, el sistema

1367
02:12:05,940 --> 02:12:16,180
salen más. Y si tenía preparado el sistema en una, le aplico a Hadamard, el sistema que

1368
02:12:16,180 --> 02:12:24,400
ha de menos. Entonces esto es lo que yo ponía antes de que uno tiene el estado inicial y

1369
02:12:24,500 --> 02:12:30,781
bajo la acción de la unitaria tiene un estado final, el más, por ejemplo. Entonces fíjense

1370
02:12:30,780 --> 02:12:38,180
lo que hizo Hadamard, Partimos de un estado que era el 0, lo voy a escribir acá en el

1371
02:12:46,380 --> 02:13:03,280
el 0 era auto vector de sigma z de autovalor, autovalor igual a 1, si yo aplico jambord obtengo

1372
02:13:03,300 --> 02:13:14,280
más y lo dejé en un auto vector de sigma x con auto valor 1.

1373
02:13:15,160 --> 02:13:15,240
Ok?

1374
02:13:17,380 --> 02:13:25,540
Y este más es una superposición porque es 1/2, este es un goto de Schrodinger por 0 + 1/2

1375
02:13:25,560 --> 02:13:25,980
por 1.

1376
02:13:26,180 --> 02:13:26,400
Ok?

1377
02:13:30,040 --> 02:13:36,060
¿Qué sería esto físicamente? Por ejemplo, sería bueno que tengo al sistema cuántico

1378
02:13:36,880 --> 02:13:46,380
preparado en cero, le hago algo, qué sé yo, le tiro con un rayo, no sé, lo que sea,

1379
02:13:46,440 --> 02:13:55,060
un rayo laser y ahora lo modifique y lo deje en un estado que es cero más uno, ¿sabes

1380
02:13:55,060 --> 02:13:56,320
raíz de 2, ¿ok?

1381
02:13:59,400 --> 02:14:00,920
¿Hagó una pregunta? ¿Se entiende esto?

1382
02:14:03,280 --> 02:14:07,880
Este sería el circuito más sencillo que pueden imaginar, el circuito cuántico, ¿no?

1383
02:14:14,040 --> 02:14:18,660
Bueno, y les dejo como ejercicio comprobar esto que les pongo acá, ¿sí?

1384
02:14:20,940 --> 02:14:24,880
lo dejo como ejercicio comprobar esto, que h0 es más, h1 es menos

1385
02:14:25,700 --> 02:14:28,180
y que h al cuadrado es la matriz identidad

1386
02:14:29,380 --> 02:14:32,000
es decir, que si vuelven, ¿qué quiere decir eso?

1387
02:14:36,160 --> 02:14:39,700
que se hacen h por 0, les da más

1388
02:14:41,100 --> 02:14:46,541
y que se hacen h por más, es h por h por 0

1389
02:14:50,460 --> 02:14:56,940
esto va a dar 0. ¿Por qué? Porque h por h es h cuadrado y h cuadrado es igual a 1, ok?

1390
02:14:58,940 --> 02:15:03,940
Del mismo modo, h por menos es igual a 1.

1391
02:15:05,340 --> 02:15:12,280
Y esto tiene que ver con que pueden comprobar que h daga es igual a h.

1392
02:15:13,670 --> 02:15:19,320
Y h, como es una comporta lógica, tiene que ser unitaria.

1393
02:15:19,320 --> 02:15:24,240
Entonces, "h" por "h" haga, esto va a dar la identidad.

1394
02:15:27,880 --> 02:15:34,020
Todo esto lo tiene que hacer como ejercicio, lo tiene que reproducir en lápiz y papel en su casa.

1395
02:15:36,420 --> 02:15:42,960
O también, equivalentemente, mejor aún si también lo hacen en Python,

1396
02:15:43,740 --> 02:15:46,760
con lo que le vamos a ir enseñando durante las próximas clases.

1397
02:15:48,000 --> 02:15:48,680
Bien, seguimos.

1398
02:15:50,320 --> 02:15:50,960
Otra compuerta.

1399
02:15:51,420 --> 02:15:52,720
Ah, bueno, y acá, notación.

1400
02:15:53,060 --> 02:15:54,220
Esto es lo que veíamos antes.

1401
02:15:55,700 --> 02:15:56,760
0 tensor 0.

1402
02:15:56,920 --> 02:15:57,740
Ya vimos que era.

1403
02:15:58,620 --> 02:16:01,440
Representaba un estado cuántico de 2 qubits.

1404
02:16:03,360 --> 02:16:06,180
Y para ahorrar notación, porque después se va a volver en

1405
02:16:06,300 --> 02:16:10,240
gorroso, vamos a poner directamente 0, 0.

1406
02:16:11,500 --> 02:16:11,900
0, 0.

1407
02:16:13,760 --> 02:16:22,540
es decir, el 0,0 es una abreviación de 0 tensor 0, a veces le vamos a poner así o a

1408
02:16:22,620 --> 02:16:28,240
veces le vamos a poner así, depende, depende la conveniencia y que como queda más fácil

1409
02:16:28,250 --> 02:16:38,899
la secuación. Y lo mismo tenemos una interpretación similar para 0,1,1,0 y 1,1. Y así calculábamos

1410
02:16:38,900 --> 02:16:42,740
el producto tensorial para combinaciones lineales.

1411
02:16:44,099 --> 02:16:47,860
Esto también les dejo como ejercicio repetirlo en casa.

1412
02:16:52,240 --> 02:16:57,200
Bien, ahora vamos a hacer algo, vamos a hacer un circuito.

1413
02:16:58,420 --> 02:17:03,480
¿Qué hace? Le aplica H al primer qubit y H al segundo qubit.

1414
02:17:03,719 --> 02:17:07,519
Fíjense que acá, déjenme escribir en la pantalla,

1415
02:17:10,040 --> 02:17:23,460
Acá tengo un producto tensorial entre matrices. Así como definían producto tensorial entre vectores, pueden definir producto tensorial entre matrices. Se hace parecido.

1416
02:17:24,240 --> 02:17:30,880
Bien, pero lo que nos importa ahora es que cómo opera esto. Acá tengo dos lugares,

1417
02:17:31,800 --> 02:17:37,400
a la izquierda y a la derecha del producto de tensorial, o cada qubit tiene su lugar.

1418
02:17:37,599 --> 02:17:40,820
Este es el qubit 1 y este es el qubit 2, castel 1 y castel 2.

1419
02:17:41,040 --> 02:17:47,019
Entonces, esta H opera sobre el qubit 1 y esta otra H opera sobre el qubit 2.

1420
02:17:47,019 --> 02:17:55,719
ok? Entonces, esto de acá quiere decir aplíqueme hadamar a cada uno de los qubits y eso es lo que

1421
02:17:55,740 --> 02:18:07,880
tengo acá, h por 0 y h por 0 y después tengo que hacer el tensor ¿no? siga, entonces h tensor h

1422
02:18:08,120 --> 02:18:14,579
aplicado a 0 tensor de 0 quiere decir aplíqueme h al primer qubit y al segundo qubit, que es lo que tengo

1423
02:18:14,580 --> 02:18:24,580
nota. Entonces ahí, ahí me queda lo que calculamos antes, lo que calculamos en la diapositiva

1424
02:18:24,719 --> 02:18:34,260
anterior que es más, más, más tensor más. Esta es una operación típica de muchos

1425
02:18:34,380 --> 02:18:35,240
al logaritmos cuántico.

1426
02:18:41,580 --> 02:18:46,519
Bueno, cuando hacen esto y hacen algo parecido a lo que puse

1427
02:18:46,519 --> 02:18:49,460
en la diapositiva anterior, si fíjense que acá tengo dos

1428
02:18:49,519 --> 02:18:51,820
combinaciones lineales, hago todos contra todos,

1429
02:18:53,420 --> 02:18:57,280
cuando hacen esto, les queda que aplicar Hadamard a cada uno

1430
02:18:57,280 --> 02:18:59,860
de los qubits, les termina dando este estado.

1431
02:19:00,500 --> 02:19:05,860
Y este estado es como un gato de Schrodinger de dos qubits,

1432
02:19:06,219 --> 02:19:09,360
porque tienen una superposición de todas las posibilidades.

1433
02:19:10,719 --> 02:19:11,840
¿Cómo es este circuito?

1434
02:19:12,740 --> 02:19:13,460
Dejenme escribir ahora.

1435
02:19:20,260 --> 02:19:24,000
Este circuito es-- tengo el primer qubit en cero,

1436
02:19:24,760 --> 02:19:25,980
al segundo qubit en cero.

1437
02:19:26,940 --> 02:19:29,639
hago Hadamard en el primero y Hadamard en el segundo.

1438
02:19:30,870 --> 02:19:33,960
Es el circuito también, el circuito más sencillo del

1439
02:19:34,000 --> 02:19:34,280
mundo.

1440
02:19:35,210 --> 02:19:39,059
Y en general, lo que van a tener al principio de muchos

1441
02:19:39,260 --> 02:19:41,960
algoritmos es Hadamard, Hadamard en todos.

1442
02:19:43,500 --> 02:19:45,540
Porque este estado, ya lo vamos a ver después,

1443
02:19:46,900 --> 02:19:50,960
esta acción lo que hace es generar un estado que es

1444
02:19:51,060 --> 02:19:54,220
superposición de todos los elementos de la base

1445
02:19:54,320 --> 02:19:55,000
computacional.

1446
02:19:55,340 --> 02:20:00,120
es como una especie de dado equiprobable sobre los elementos de la base

1447
02:20:00,200 --> 02:20:04,060
de computación. Entonces este es otro ejemplo todavía de circuito cuántico.

1448
02:20:04,270 --> 02:20:09,520
¿Está bien? Pues ven que ya con todas estas herramientas vamos avanzando.

1449
02:20:11,680 --> 02:20:17,180
En este estado particular, si ustedes midieran, si miden sigma z, es decir,

1450
02:20:17,240 --> 02:20:21,360
si hacen un experimento y miden sigma z para cada uno de los qubits,

1451
02:20:21,940 --> 02:20:26,740
Lo que van a obtener es que cada output de la base computacional

1452
02:20:27,140 --> 02:20:28,320
ocurre con probabilidad de un cuarto.

1453
02:20:29,280 --> 02:20:29,580
¿Por qué?

1454
02:20:29,660 --> 02:20:32,340
Porque cada uno de estos tiene coeficiente 1/2.

1455
02:20:33,780 --> 02:20:37,840
Cuando miden, va a tener que la probabilidad de obtener que

1456
02:20:37,880 --> 02:20:42,220
se yo, el 0, 0 es 1/2 al cuadrado.

1457
02:20:43,640 --> 02:20:49,860
Es decir, p 0, 0 es p de 1, 0 es igual a p 0, 1,

1458
02:20:50,060 --> 02:20:52,520
y va la p de 1 a 1 y todo da un cuarto.

1459
02:20:53,039 --> 02:20:57,040
Entonces, esta operatoria de aplicar hammer a cada uno de los

1460
02:20:57,240 --> 02:21:06,000
qubits da un estado que cuando miden les puede dar 0,0 o 0,1 o 1,0 o 1,1,1,

1461
02:21:06,040 --> 02:21:07,140
todos con probabilidad un cuarto.

1462
02:21:08,580 --> 02:21:11,660
Claro que al ser 4, además suman 1 entre los 4.

1463
02:21:12,860 --> 02:21:13,780
Exacto, exacto.

1464
02:21:14,460 --> 02:21:19,059
Fijate que, sí, suma de--

1465
02:21:19,060 --> 02:21:21,220
es una volu de espero, lo hago porque es importante, ¿no?

1466
02:21:21,340 --> 02:21:27,980
Es decir, módulo de un medio al cuadrado más módulo de un medio al cuadrado más módulo

1467
02:21:28,240 --> 02:21:32,840
de un medio al cuadrado más módulo de un medio al cuadrado es igual a 1.

1468
02:21:33,300 --> 02:21:37,920
Esto es lo que le ponía antes, que alfa 1 módulo alfa 1 al cuadrado más módulo alfa

1469
02:21:38,040 --> 02:21:40,440
2 al cuadrado, etcétera, y igual a 1, ¿te acordás?

1470
02:21:41,200 --> 02:21:44,080
Bueno, acá es esto, lo que pasa que acá es equiperebable.

1471
02:21:45,600 --> 02:21:52,680
bien, sí, bueno otra compuerta importante es la compuerta x, ya vamos a ver que esta

1472
02:21:52,940 --> 02:21:59,200
después la podemos usar para medir en la dirección x justamente y ustedes pueden comprobar que

1473
02:21:59,880 --> 02:22:04,940
esta es como una especie de no, porque lo que hace es x contra 0 de a 1 y x contra 1

1474
02:22:04,980 --> 02:22:15,660
0 sería como el análogo del note, del note clásico en la computadora cuántica y de

1475
02:22:15,780 --> 02:22:20,080
vuelta utilizamos una notación similar para el circuitito, un circuitito muy

1476
02:22:20,240 --> 02:22:26,200
sencillo tiene un qubit y sobre ese qubit aplico la compuerta not, después

1477
02:22:26,320 --> 02:22:32,818
está la compuerta y que tiene una acción muy similar al note nada más que

1478
02:22:32,820 --> 02:22:39,280
ahora les agrega una fase compleja fíjense que acá estas fases complejas van a ser importantes

1479
02:22:40,220 --> 02:22:47,840
al final del día, es decir no está adornos el número complejo, porque si fuera un solo

1480
02:22:47,920 --> 02:22:53,360
qubit no haría nada pero cuando lo combinen con comportas que ahora vamos a ver comportas

1481
02:22:53,400 --> 02:22:58,800
que entrelazan a los qubits, es decir comportas que hacen interactuar a los qubits entre sí,

1482
02:22:59,620 --> 02:23:07,440
vamos a ver una. Ok, y esta es la matriz. Es que sé que coincide con la matriz de Pauli y.

1483
02:23:10,560 --> 02:23:16,960
Bien, y esta es la compuerta lógica z, pueden ustedes calcular lo que hace en la base computacional

1484
02:23:17,200 --> 02:23:23,020
y así siguiendo. Bueno, acá parece la primera compuerta interesante de dos qubits, la compuerta

1485
02:23:23,020 --> 02:23:32,360
si noto o control noto que se denota con este circuitito yo estoy usando cubit 1 cubit 2

1486
02:23:32,540 --> 02:23:41,140
pero en general en computación cuántica es como python no es número empieza a contar por 0 cuido

1487
02:23:41,240 --> 02:23:51,220
0 y cubit 1 cuido 1 cuido 2 cuido n no importa es una volubés pero a veces voy a contar desde 1

1488
02:23:51,220 --> 02:23:58,800
a veces voy a ocultar desde cero, pero bueno, sepanlo. Lo importante es que bueno, este es

1489
02:23:58,800 --> 02:24:04,060
un circuito donde aplicamos la comporta control note. Y esta control note es una comporta

1490
02:24:04,180 --> 02:24:15,120
de dos qubits. Fíjense que esto es una matriz, pera en qué le he escrito acá. Esto pertenece

1491
02:24:15,120 --> 02:24:26,020
c a la 4 por 4. Entonces, cnut de dónde opera? Manda vectores de c a la 4 a vectores de c a la 4.

1492
02:24:26,290 --> 02:24:39,340
Es decir, para poder hacer el producto de esta matriz por algo acá, ustedes acá tienen que meter a un vector de c4,

1493
02:24:39,620 --> 02:24:45,620
una alfa 1, alfa 2, alfa 3, alfa 4. Si no nos dan los números, entienden, uno tiene que hacer esto por esto.

1494
02:24:45,840 --> 02:24:48,100
Si no nos dan el tamaño de las matrices para multiplicarse.

1495
02:24:49,220 --> 02:24:51,440
Entonces, esta es sí o sí

1496
02:24:52,420 --> 02:24:55,700
una comporta que opera sobre un espacio de 2 qubits

1497
02:24:56,560 --> 02:25:00,260
y se conoce como una comporta entre las antes. Ahora van a ver por qué.

1498
02:25:02,380 --> 02:25:06,280
Bueno, esto es lo que les decía antes. Aquí está opera sobre 2 qubits.

1499
02:25:07,620 --> 02:25:10,680
Ah, y perdón, esta es la representación matricial.

1500
02:25:11,090 --> 02:25:17,120
Y está bueno ver cómo opera C-NOT en la base computacional.

1501
02:25:17,400 --> 02:25:18,540
¿Por qué se llama C-NOT?

1502
02:25:18,600 --> 02:25:19,500
Es el control-not.

1503
02:25:19,940 --> 02:25:25,040
Bien, esta es la tabla de verdad, que sería exactamente igual

1504
02:25:25,050 --> 02:25:27,480
a la tabla de verdad clásica del control-not

1505
02:25:27,580 --> 02:25:28,760
para la base computacional.

1506
02:25:28,960 --> 02:25:29,780
¿Qué quiere decir esto?

1507
02:25:29,840 --> 02:25:32,200
Bueno, lo escribo acá.

1508
02:25:32,660 --> 02:25:43,980
Esta tabla, lo que calculé es Cnought aplicada al 0, 0, Cnought aplicada al 0, 1, Cnought

1509
02:25:45,460 --> 02:25:49,220
aplicada al 1, 0 y Cnought aplicada al 1, 1.

1510
02:25:49,970 --> 02:25:51,300
Y voy calculando los output.

1511
02:25:52,020 --> 02:25:52,880
Esto lo pueden hacer.

1512
02:25:53,820 --> 02:25:55,480
Tarea, háganlo en sus casas.

1513
02:25:56,500 --> 02:25:58,200
Cnought 0, 0, 0, 0, 0, 1.

1514
02:25:59,620 --> 02:26:06,660
sería hacer por ejemplo c0 por 0,0... seria hacer

1515
02:26:29,620 --> 02:26:37,460
y esto les va a dar otro vector de 4, hazlo, haz la cuenta y lo mismo para 0 1 1 0

1516
02:26:40,400 --> 02:26:45,740
acá en este, lo escribimos, 0 0 1 0

1517
02:26:49,620 --> 02:26:51,540
ahora si lo puse bien, no? si

1518
02:26:53,020 --> 02:26:53,220
bien

1519
02:26:57,040 --> 02:27:06,380
sí, ¿ven? esta es la cn, si acá lo pongo más claro, supongan que multiplicaron la misma cn

1520
02:27:07,570 --> 02:27:15,440
por el vector que se yo, el 0,1 bueno, eso tendrían que hacer

1521
02:27:18,580 --> 02:27:31,220
pero 1 0 por 0 1 0 0, este tiene 0 0 1 0, bueno y ve en el resultado y así, y si fuera

1522
02:27:32,160 --> 02:27:40,920
el 1 1 sería el 0 0 0 1, bien entonces tienen que como ejercicio calcular esta tabla de

1523
02:27:40,940 --> 02:27:48,120
verdad entonces si el primer qubit está en cero y el segundo voy a la primera a la primera línea de la

1524
02:27:50,820 --> 02:27:55,260
a la primera línea no si el primer qubit está en cero y el segundo está en cero esto serían los

1525
02:27:55,460 --> 02:28:01,780
inputs pueden comprobar que quedan los dos igual cuando aplican senot es decir si los dos están

1526
02:28:02,040 --> 02:28:07,700
cero cero no cambia nada si el primero está en cero y el segundo está en uno tampoco cambia

1527
02:28:07,700 --> 02:28:13,220
nada, pueden comprobarlo. Ahora, si el primero está en 1, lo cual quiere decir que está,

1528
02:28:13,560 --> 02:28:20,960
digamos, activado, por eso el 1 es el qubit control, ¿sí? Tengo el qubit 0 y el qubit

1529
02:28:21,100 --> 02:28:30,200
1. Entonces, el primero es el control y el segundo qubit es el target. Entonces, si

1530
02:28:30,260 --> 02:28:36,500
el primero está en 1, ahora el control node niega al segundo. Es decir, si tengo 1 0 pasa

1531
02:28:36,500 --> 02:28:44,100
a 1,1 y si tengo 1,1 pasa a 1,0. Es decir, si el primer qubit está activado, el segundo qubit

1532
02:28:44,140 --> 02:28:49,680
se niega. Eso es lo que hace control. Ahora, si el primer qubit no está activado, si está

1533
02:28:49,760 --> 02:28:56,340
en 0, todo que hay igual. El segundo qubit, pues eso es un control. El primer qubit actúa

1534
02:28:56,380 --> 02:29:02,400
como control y el segundo qubit actúa como objetivo o target. Tiene la compuerta control.

1535
02:29:03,340 --> 02:29:10,540
en un análogo clásico, pero bueno en cuántica da lugar a novedades porque acá viene lo interesante.

1536
02:29:12,240 --> 02:29:19,100
Acabamos de hacer un circuitito, lo voy a escribir arriba después. El circuitito primero

1537
02:29:19,100 --> 02:29:25,920
le aplicábamos "Hammard" al primer qubits, el segundo no le hacemos nada. Esto me da

1538
02:29:25,940 --> 02:29:34,640
este estado y quede en este estado y qué pasa si ahora aplico sinot a todo esto, si

1539
02:29:34,680 --> 02:29:43,720
aplico sinot recuerden que todas estas actúan por multiplicación matricial como tal son

1540
02:29:43,780 --> 02:29:50,540
operadores lineales entonces sinot por esto es sinot por este más sinot por este, se

1541
02:29:50,540 --> 02:29:54,320
se distribuye, entonces voy a hacer sinot 0,0, sinot 0,1.

1542
02:29:55,500 --> 02:29:58,280
Acá puedo utilizar la tabla de verdad,

1543
02:30:00,180 --> 02:30:02,500
toque hacer sinot 0,0, sinot 0,1.

1544
02:30:04,220 --> 02:30:07,500
Si me fijo la tabla de verdad, sinot 0,0, no cambia nada,

1545
02:30:08,320 --> 02:30:12,900
pero sinot 1,0, sí cambia porque el 1 está activado, el primer qubit.

1546
02:30:13,520 --> 02:30:15,080
Entonces el 2 se tiene que negar,

1547
02:30:15,540 --> 02:30:24,500
así calculan cuánto vale esto y este estado era el que yo les decía antes que estaba entrelazado

1548
02:30:25,360 --> 02:30:31,460
y este es el que tiene que no se puede escribir como producto tensorial de estados los qubits por

1549
02:30:31,520 --> 02:30:40,620
separado, entonces este estado no es separable es entrelazado, les dejo como ejercicio probar esto,

1550
02:30:40,660 --> 02:30:56,640
es fácil probarlo. ¿Cómo probarían que uno se reíe de 2 por 0,0 más 1,1? No se

1551
02:30:56,640 --> 02:31:06,260
puede escribir como un producto tensorial, bueno, hagan alfa 1 por si 1, no, perdón,

1552
02:31:08,640 --> 02:31:20,740
tienen que hacer alfa 1 por 0 más alfa 2 por 1, producto tensorial beta 1 por 0 más beta

1553
02:31:20,780 --> 02:31:30,000
1 por 1 y lo igualan y van a ver que no existe ninguna combinación de alfa 1, alfa 2 y beta

1554
02:31:30,060 --> 02:31:34,880
1 y beta 2 que haga esto. Se van a ver que ya en un sistema de ecuación es inconsistente.

1555
02:31:35,420 --> 02:31:47,080
Haganlo como ejercicio y se van a convencer de que este estado no es separable. Bien,

1556
02:31:47,180 --> 02:31:54,980
bien y a ver si lo tengo acá, bueno, ¿cómo es el circuito? porque acá lo escribí en

1557
02:31:55,000 --> 02:32:00,740
términos de multiplicaciones de matrices ¿no? ¿cómo sería el circuito de esto? tengo,

1558
02:32:02,000 --> 02:32:11,279
lo voy a escribir a un costado acá en la esquina. Esta ecuación de acá me dice "aplique

1559
02:32:11,280 --> 02:32:15,840
"h" "jabamar" al cero y al otro no le haga nada, entonces al primer qubit, perdón.

1560
02:32:16,920 --> 02:32:22,600
Entonces tengo el qubit cero y el qubit uno, los dos están en cero al principio,

1561
02:32:24,880 --> 02:32:28,400
entonces al primero le aplico "jabamar" y al segundo no le haga nada.

1562
02:32:29,500 --> 02:32:31,720
Y luego le aplico "sinot" a los dos.

1563
02:32:32,780 --> 02:32:36,600
Acá a la salida hay un primer estado, que es este de acá,

1564
02:32:37,280 --> 02:32:42,680
Este de acá es el estado de la salida de la primera operación y en la segunda utilizo

1565
02:32:42,680 --> 02:32:45,080
el primero como control y el segundo como target.

1566
02:32:47,680 --> 02:32:50,900
Y a la salida tengo este estado de acá.

1567
02:32:53,640 --> 02:33:01,700
Este es un ejemplo de un circuito cuántico que combina a Hadamard y Sinot y me deja como

1568
02:33:01,700 --> 02:33:04,740
resultado a los dos qubits en un estado entrelazado.

1569
02:33:11,200 --> 02:33:14,360
Bueno, ¿y qué pasa en un estado entrelazado? ¿Cómo lo tenemos que pensar?

1570
02:33:14,660 --> 02:33:19,960
Bueno, supongamos que tenemos a una gente, a la gente azul,

1571
02:33:20,680 --> 02:33:25,320
midiendo en el primer qubit y a la gente rojo midiendo el segundo qubit.

1572
02:33:26,300 --> 02:33:40,040
Bueno, cada qubit puede dar 0 o 1, piensen que estamos en la base computacional, los resultados son 0 y 1, o 0 o 1 o 1 o 0, vamos midiendo.

1573
02:33:41,720 --> 02:33:50,060
Y la idea es que cuando tenemos este circuito que era el que les dibujaba antes, primero aplico "hammer" al primer qubit y después "ctrl" "note" entre el primero y el segundo,

1574
02:33:53,720 --> 02:33:56,720
Acá está, ven que hay dos formas de expresarlo esto.

1575
02:34:01,500 --> 02:34:08,060
Hay dos formas de expresarlo, o les presa así en términos de circuitos, o les presa así en términos de una formulita.

1576
02:34:09,640 --> 02:34:15,020
Las dos fórmulas son válidas, son equivalentes. A veces conviene ver más las cosas como circuito,

1577
02:34:16,600 --> 02:34:22,360
a veces comienzan a ver más las cosas como fórmulas. Ahora, sin miedo en la base computacional,

1578
02:34:23,760 --> 02:34:32,240
sin miedo en la base computacional, solo voy a observar 00 y 11, lo cual indica que los

1579
02:34:32,440 --> 02:34:45,680
qubits están correlacionados. Esperen, que vuelvo a las posibilidades, ahí está. Esto

1580
02:34:46,260 --> 02:34:52,420
O observo 0,0 o observo 1,1, pero no voy a observar el 0,1 o 1,0.

1581
02:34:52,860 --> 02:34:57,580
Igual, no estoy explicando completamente la noción de correlaciones,

1582
02:34:57,800 --> 02:34:59,480
estoy simplemente intentando dar una idea.

1583
02:35:00,400 --> 02:35:02,420
De esto lo vamos a seguir viendo en las futuras clases.

1584
02:35:06,120 --> 02:35:11,360
También se puede preparar el estado que se conoce como singlete,

1585
02:35:15,400 --> 02:35:23,060
y si preparo este sólo voy a observar el 01 y el 10. Este también es

1586
02:35:23,120 --> 02:35:29,360
entrelasado, este estaba muy importante porque es uno de los que viola

1587
02:35:29,700 --> 02:35:34,860
maximalmente la desigualdad de Clause Horn, Schimony Hall. Piensen que hace un

1588
02:35:34,880 --> 02:35:46,820
un par de años se otorgó un plemionóvel por esto, digamos, por la realización de los

1589
02:35:48,439 --> 02:35:53,540
primeros experimentos en violación del que se conoce como desigualdades de Bell, que

1590
02:35:53,580 --> 02:36:00,479
es algo que vamos a ver en el curso también. Pero bueno, la idea es que en una computadora

1591
02:36:00,480 --> 02:36:14,320
cuántica pueden preparar este tipo de estados, me mata, hay una pregunta sobre esto, acá

1592
02:36:14,580 --> 02:36:20,680
lo que les dije es, bueno, este es si quieren el primer ejemplo del circuito cuántico que

1593
02:36:20,700 --> 02:36:27,560
vienen sus vidas, después vamos a hacer esto con Python en un simulador de computadora cuántica,

1594
02:36:28,840 --> 02:36:33,040
y después lo vamos a hacer en una computadora cuántica de verdad, ¿tabian?

1595
02:36:38,860 --> 02:36:42,260
pero la idea es que los circuitos van a ser como esto, ¿no?

1596
02:36:43,800 --> 02:36:44,740
en general van a tener

1597
02:36:48,220 --> 02:36:48,880
n qubits

1598
02:36:51,460 --> 02:36:55,560
y sobre los n qubits van a aplicar compuertas

1599
02:36:55,560 --> 02:37:03,020
básicamente los NQBs van a aplicar una familia de operaciones unitarias que va a dar una

1600
02:37:03,720 --> 02:37:08,460
familia de operaciones unitarias y a la salida van a medir todos los QBs, esa es la idea,

1601
02:37:09,080 --> 02:37:14,300
de un circuito cuántico. Y los algoritmos cuánticos se van a escribir así como circuitos

1602
02:37:14,320 --> 02:37:24,760
cuánticos. Fíjense que yo estoy explicando las cosas en el bajo nivel absoluto, es decir,

1603
02:37:24,840 --> 02:37:31,380
estamos viendo cómo son los circuitos cuánticos a nivel con puertas

1604
02:37:32,480 --> 02:37:44,120
elementales. Bien, ahora no, pero vamos a ver en las próximas clases cómo

1605
02:37:44,200 --> 02:37:47,880
preparar circuitos, cómo programar circuitos cuánticos con distintas

1606
02:37:48,040 --> 02:37:53,000
plataformas de desarrollo software. En esta materia nos vamos a vamos a usar

1607
02:37:53,000 --> 02:38:00,540
Kiskit y vamos a usar Amazon Bracket. Los que ya tengan Python o los que logran

1608
02:38:00,720 --> 02:38:05,580
instalar ese Python ya se pueden ir armando entornos, un entorno para Kiskit,

1609
02:38:05,810 --> 02:38:13,520
otro entorno para Amazon Bracket, así después no es más fácil ir haciendo

1610
02:38:13,520 --> 02:38:19,100
las cosas. Paren que se me suele porque apreté sin querer el botoncito.

1611
02:38:21,040 --> 02:38:21,720
mmm

1612
02:38:30,680 --> 02:38:35,400
Just once, ok, bien, sigo.

1613
02:38:40,000 --> 02:38:40,800
Bueno, preguntas.

1614
02:38:43,200 --> 02:38:48,480
Esto de... entiendo que no es fácil, pero al mismo tiempo debería ser claro, ¿no?

1615
02:38:49,470 --> 02:38:50,100
Me parece.

1616
02:38:51,400 --> 02:38:55,420
Bien, sigo con ejemplos de comportas lógicas cuánticas

1617
02:38:57,080 --> 02:38:57,580
hasta terminar.

1618
02:38:58,730 --> 02:39:03,040
Hay otra comporta que es conocida, que es el SWAP, que permite intercambiar

1619
02:39:03,040 --> 02:39:07,820
cambiar el estado, los estados por ejemplo, el swap del 0, 0, nada, no cambia nada, pero

1620
02:39:07,860 --> 02:39:16,380
el swap del 0, 1 me manda al 1, 0 y el swap del 1, 0 me manda al 0, 1, si, lo que haces

1621
02:39:17,260 --> 02:39:23,540
intercambiar estados cuánticos, el símbolo lógico de esta compuerta es esto, como digamos

1622
02:39:23,640 --> 02:39:28,780
dos cruces con una flechita que las une, esta también es una compuerta de dos qubits, así

1623
02:39:28,780 --> 02:39:37,520
así como hay comportas de dos qubits, hay comportas de tres qubits, uff, pero sigo conectado,

1624
02:39:37,620 --> 02:39:47,720
sí, no? Sí, sí, sí, perfecto, y sigo compartiendo el pantalla. Un ejemplo de comporta de tres

1625
02:39:47,780 --> 02:39:56,420
qubits es Topholi, Topholi también tiene un análogo clásico, está opera en un espacio

1626
02:39:56,420 --> 02:40:04,480
de Dimension 8, el símbolo de Tosfoli es este de acá, si o si tienen que meter acá un

1627
02:40:04,620 --> 02:40:15,560
vector de 8 componentes, tiene alfa 1, alfa 2 hasta el alfa 8, o podría empezar a contar

1628
02:40:15,640 --> 02:40:24,800
de 0 alfa 0 alfa 1 hasta alfa 7. Entonces este va a ser un estado cuántico general de

1629
02:40:26,200 --> 02:40:31,020
c a la 2 al cubo, perdón, 2 a la 8 puse.

1630
02:40:33,920 --> 02:40:39,840
¿Qué sería c a la 8? ¿Qué sería el espacio de estado de 3 qubits? Entonces,

1631
02:40:41,320 --> 02:40:43,520
bueno, Tófoli actúa en este espacio.

1632
02:40:45,860 --> 02:40:50,400
y este es el símbolo lógico y tiene la siguiente tabla de verdad.

1633
02:40:51,850 --> 02:40:57,560
Esta es más complicada que control not porque es el doble control not y qué hace tofoli.

1634
02:40:57,720 --> 02:41:06,120
Bueno, básicamente si los dos primeros, si alguno de los dos primeros están,

1635
02:41:11,080 --> 02:41:18,479
digamos hasta acá no cambia nada en estas primeras 4 2 4 5 líneas

1636
02:41:22,560 --> 02:41:26,540
1 0 0 en estas primeras 5 líneas no cambia nada

1637
02:41:28,800 --> 02:41:36,720
pero en las dos últimas si cambia si los dos primeros que están activados lo que hace es negar

1638
02:41:36,720 --> 02:41:43,080
el tercero, por ejemplo al 1, 1, 0 la manda al 1, 1, 1 y al 1, 1, 1 lo manda al 1, 1, 1, 0

1639
02:41:43,960 --> 02:41:51,220
es el doble control node por decirlo de una manera y se puede escribir esto matemáticamente

1640
02:41:51,360 --> 02:41:57,860
de forma elegante así, a esto lo vamos a ver, esta es la suma módulo 2, ¿cómo es la

1641
02:41:57,860 --> 02:42:14,360
suma módulo 2 bueno 0 módulo 2 0 es igual a 0, 0 módulo 2 1 es igual a 1, 1 módulo 2 es 0 es igual a 1 y 1 módulo 2 1 y acá es lo único que cambia

1642
02:42:14,380 --> 02:42:27,260
vuelve a dar 0, típicamente 1+1 es 2, pero no, acá 1 módulo 2 1 0, es decir para 0, 0, 0, 1 y 1, 0

1643
02:42:27,540 --> 02:42:34,880
la suma módulo 2 da igual que siempre, pero cuando ponen 1 y 1 da 0, es como un reloj,

1644
02:42:35,839 --> 02:42:38,260
cuando da la vuelta vuelvo a empezar

1645
02:42:42,100 --> 02:42:45,060
bueno esto recuerdenlo le voy a explicar de vuelta más adelante pero

1646
02:42:45,760 --> 02:42:48,960
tenga lo en mente porque le vamos a usar de forma cada vez más complicada

1647
02:42:49,580 --> 02:42:52,120
a lo largo del curso y este es simplemente el producto

1648
02:42:52,420 --> 02:42:56,300
el producto de bits 0x00, 0x10

1649
02:42:58,460 --> 02:43:00,420
1x00 y 1x1, ¿sí?

1650
02:43:08,200 --> 02:43:14,180
Bueno, y después hay otra, con puerta lógica, que es la compuerta de Fredking, está también

1651
02:43:14,280 --> 02:43:19,500
desconocida, no es tan conocida como las otras, pero es el control swap básicamente.

1652
02:43:22,620 --> 02:43:30,580
Bueno, y no confundir porque cuando la gente se comunica, puede usar el concepto de lógica

1653
02:43:30,640 --> 02:43:38,700
cuántica en distintos sentidos y ambos sentidos están bastante establecidos en comunidades

1654
02:43:39,710 --> 02:43:43,620
que tienen intersección pero son completamente distintas.

1655
02:43:44,880 --> 02:43:50,660
Una cosa es la lógica cuántica en el sentido de la lógica cuántica de Birkhoff y von Neumann,

1656
02:43:50,730 --> 02:43:59,000
que es una especie de rama de la física matemática, que se encarga de establecer si quieren cuál

1657
02:43:59,000 --> 02:44:00,560
es la lógica de la cuántica.

1658
02:44:01,630 --> 02:44:06,960
Y otro sentido es el conjunto de comportas lógicas cuánticas y sus propiedades en el

1659
02:44:06,980 --> 02:44:08,560
contexto de la computación cuántica.

1660
02:44:09,580 --> 02:44:15,040
no puede por supuesto mezclar estas dos áreas del conocimiento, yo lo he hecho, es como

1661
02:44:15,620 --> 02:44:24,240
una de mis áreas, de investigación, pero por ejemplo en este paper de Nature dice "Lógica

1662
02:44:24,300 --> 02:44:31,220
cuántica de tres qubits de un fotón usando moduladores de luz espaciales, lo que hicieron

1663
02:44:31,260 --> 02:44:40,040
acá es aplicar o implementar con puertas lógicas cuánticas en tres qubits utilizando

1664
02:44:40,980 --> 02:44:49,180
moduladores de luz espaciales y otra cosa es lógica cuántica en este sentido esto no lo

1665
02:44:49,280 --> 02:44:54,540
vamos a ver en el curso la lógica cuántica a quien le interese le pudo pasar muchos libros de esto

1666
02:44:57,060 --> 02:45:01,240
pero bueno nosotros vamos a usar el concepto de lógica cuántica en este sentido de acá

1667
02:45:01,240 --> 02:45:04,420
Bueno, y con esto termino la clase de hoy.

1668
02:45:07,060 --> 02:45:16,980
Dejo de compartir y nos quedan unos pocos minutitos para preguntar, pero los veo ya medio mortos, veo que ya me de preguntar nada, con lo cual quiere decir que están cansados.

1669
02:45:17,320 --> 02:45:28,360
Pero queda todo grabado, así que les invito a ver los vídeos, a ver el vídeo y a repetir todas las cosas que yo fui haciendo en lápiz y papel.

1670
02:45:29,860 --> 02:45:38,780
y a los que les del cuero, a los también Paito. Bien, preguntas, si no, por ella vamos cerrando

1671
02:45:38,780 --> 02:45:47,340
el boliche. Yo tengo una consulta más administrativa, ¿quedan cinco clases? ¿Cualquiero que eran

1672
02:45:47,400 --> 02:45:56,260
diez? Seis clases, seis clases, seis clases. Ok. Pero es probable que metamos un par de

1673
02:45:56,260 --> 02:46:04,340
es más de bonus track. No es flexible pero para quienes quieran, uno cuando se

1674
02:46:04,420 --> 02:46:11,720
inscribe tiene un compromiso, pero para completar si queda algo volando por ahí

1675
02:46:12,000 --> 02:46:17,440
para completar es probable que metemos un par de clases más de bonus track para

1676
02:46:17,500 --> 02:46:23,979
meter algunos temas que nos hayan visto, para profundizar pero me parece que

1677
02:46:23,980 --> 02:46:31,000
vamos bastante bien en el siguiente sentido ustedes tienen todo grabado y van a tener

1678
02:46:31,440 --> 02:46:36,540
las diapositivas de las cuatro primeras clases es un montón de material y tienen los libros

1679
02:46:37,900 --> 02:46:43,400
pueden ver los videos una y otra vez entonces mi invitación es que hagan eso que traten

1680
02:46:43,400 --> 02:46:49,620
de repetir todo con lápiz y papel y traten de ir aprendiendo todo lo que pueda para poder

1681
02:46:49,620 --> 02:46:53,340
ingresar a la segunda fase de la materia en la cual vamos a empezar a ver al

1682
02:46:53,400 --> 02:46:54,080
algoritmos cuánticos.

1683
02:46:59,560 --> 02:47:05,320
Es muy importante que intenten estar al día con la lectura y con el estudio de

1684
02:47:05,320 --> 02:47:13,320
las clases. Le puedo hacer una consulta. Nos va a detallar el entorno que usted quiere

1685
02:47:13,340 --> 02:47:19,600
en el entorno que usted quiere que trabajemos, así lo vamos instalando y demás, o...

1686
02:47:20,720 --> 02:47:27,060
- Sí, sí, instalante... -...por ejemplo, yo ya hice algunas cosas en Python, pero en colab, por ejemplo.

1687
02:47:28,720 --> 02:47:35,540
- Sí, sí. - Pero por eso quiero saber qué entorno va a ser el adecuado, en el caso de que tengamos que encontrar algo usted.

1688
02:47:36,840 --> 02:47:44,100
si, si, aceite dos entornos, uno en el cual te instales la última versión de

1689
02:47:44,260 --> 02:47:49,720
kiskit, ok, y otro en el cual te instales la última versión de bracket

1690
02:47:51,240 --> 02:47:56,220
y cuáles son los más, o sea eso usted lo va a compartir, cuáles son los mejores o lo

1691
02:47:56,420 --> 02:48:04,920
investigamos nosotros? no hay mejor entorno, yo la realidad es que para laburar por ejemplo

1692
02:48:04,920 --> 02:48:10,240
un poco porque el compañero al principio, bueno hablaba por ejemplo de Anacond y demás

1693
02:48:11,200 --> 02:48:11,620
y bueno.

1694
02:48:12,900 --> 02:48:13,620
No, no, no, pero para una cosa no.

1695
02:48:13,620 --> 02:48:16,340
Yo no lo entorno, pero ya lleva un tiempo también.

1696
02:48:16,920 --> 02:48:24,700
Una cosa es, o para para, una cosa es el programa, el software que vos utilices para

1697
02:48:26,301 --> 02:48:27,500
codear en Python.

1698
02:48:29,180 --> 02:48:34,000
vos puedes usar, por ejemplo, "BSCode", "chozoBSCode", dice ejemplo, le voy a dar con eso.

1699
02:48:36,059 --> 02:48:43,320
Pero no importa lo que vos uses, vos siempre vas a estar corriendo Python, ¿entendés?

1700
02:48:44,380 --> 02:48:44,880
Sí, sí, sí.

1701
02:48:46,220 --> 02:48:52,320
Y Python, lo que quiso explicarle, Andrés, es que vos a Python la práctica recomendada

1702
02:48:52,320 --> 02:48:56,160
es definir un entorno para cada tarea, pero son dos cosas distintas.

1703
02:48:56,160 --> 02:49:01,240
una cosa es un entorno de Python, vos el mismo entorno de Python lo puedes activar en distintas

1704
02:49:01,380 --> 02:49:12,280
plataformas, en Spider, en un Jupyter Node, en BSCode, no se deben haber miles, ¿entendés a lo que

1705
02:49:12,280 --> 02:49:19,800
voy? Entonces, vos lo que tenés que armar es en el editor que más te guste, el que vos uses para

1706
02:49:19,800 --> 02:49:27,640
trabajar en tu trabajo cotidiano, vos sos programador o algo así? Sí, estoy en una URI y la

1707
02:49:27,740 --> 02:49:33,420
Ternicatura de Programación. ¿Qué usas? ¿Qué usas? ¿Qué es ese código? No, Python generalmente y bueno ahora estamos en

1708
02:49:33,460 --> 02:49:40,980
Objetos 2 y usamos Colab por ejemplo nosotros. Bueno, ¿puedes usar Colab también? Pero en

1709
02:49:41,080 --> 02:49:46,720
Colab te vas a tener que definir un entorno de Python en el cual instales la librería

1710
02:49:47,720 --> 02:49:52,260
¿entendés? Sí, sí, yo lo, yo lo hice inclusive, y la

1711
02:49:52,280 --> 02:49:59,160
perfecto. Por eso yo quería aprender qué tan mal estaba a hacerlo ahí. No, no es que

1712
02:49:59,180 --> 02:50:05,900
está mal. Leandro, ¿por qué es un fundamentalista? Que sí yo soy el software libre, este, bueno,

1713
02:50:06,260 --> 02:50:12,160
perfecto. Está bien, pero vos usá el que quieras. Ah, listo, listo. Solo quería saber

1714
02:50:12,160 --> 02:50:18,340
eso, quizá no es el que quieras. Para un nuevo entorno vamos a ver si podemos. Para aprender

1715
02:50:18,460 --> 02:50:28,340
una cosa nueva igual para para para yo la próxima clase te lo explico modo holic que es aprueba

1716
02:50:28,420 --> 02:50:36,960
de boludos esa prueba de boludos. Me pido tranquilo porque yo te digo apretar vas a ver

1717
02:50:36,960 --> 02:50:45,640
que es no vas a tener que aprender nada nuevo, apretar acá, hacer esto, abrir unas ventanitas

1718
02:50:46,060 --> 02:50:53,920
y apretas ahí y se hace, entonces no va a haber códigos complejos, después las cuentas

1719
02:50:53,980 --> 02:51:00,120
van a ser códigos complejos, cuentas probablemente no la senten, pero la parte de abrir el editor

1720
02:51:00,160 --> 02:51:06,980
como lo abro yo es fácil esa prueba de volumen entonces no te preocupes que está bueno en

1721
02:51:06,980 --> 02:51:12,620
la prenda también por ejemplo porque porque no aprender a ver seco si es lo más fácil

1722
02:51:12,820 --> 02:51:20,160
el mundo si si también usamos ese cobus nosotros obvio que usas por eso pero si que esas son

1723
02:51:20,240 --> 02:51:27,840
en colapso yo no soy duchon colapso duchon colapso pero bueno entones le vas a poder

1724
02:51:27,840 --> 02:51:31,960
hacer todo lo que yo hago en bs, ¿cómo le vas a poder hacer en collab?

1725
02:51:34,199 --> 02:51:38,180
Yo pensaba que esa es la entrega, si tenemos que entregar un code y lo entregar en collab,

1726
02:51:38,440 --> 02:51:40,420
capaz que genera un code.

1727
02:51:40,470 --> 02:51:43,540
No, vos me vas a entregar, vos me vas a entregar una Jupyter Notebook.

1728
02:51:44,480 --> 02:51:46,380
Ah, ok, ok, entonces es Jupyter.

1729
02:51:46,620 --> 02:51:49,180
Es decir, un archivo y pnb me vas a entregar.

1730
02:51:49,400 --> 02:51:52,560
Entonces yo entiendo que vos puedes armar con... y por eso.

1731
02:51:53,320 --> 02:51:54,800
Entendés que no es un solo problema.

1732
02:51:55,840 --> 02:51:57,700
Claro, Colab general mismo.

1733
02:51:59,440 --> 02:52:03,020
Exacto, exacto, eso es lo que te estoy queriendo transmitir, todo es lo mismo, porque vos

1734
02:52:03,800 --> 02:52:06,580
son todos editores de ArchEos y PNB.

1735
02:52:06,840 --> 02:52:07,040
¿Entendés?

1736
02:52:07,920 --> 02:52:08,680
Sí, sí, sí.

1737
02:52:08,820 --> 02:52:13,660
Bueno, puedes abrir con el que quieras, pues otro que yo no conozco y está perfecto.

1738
02:52:15,859 --> 02:52:20,860
Bueno, pero quizás siempre se podría avisar el Studio Code, que ya lo tengo ahí en la

1739
02:52:20,900 --> 02:52:21,320
Compu.

1740
02:52:22,580 --> 02:52:22,800
Claro.

1741
02:52:22,960 --> 02:52:27,620
No tendría problema, pero quizás instalar anaconda y generar un nuevo entorno.

1742
02:52:28,840 --> 02:52:33,480
No dispongo quizás desde el tiempo para hacerlo ahora, me encantaría.

1743
02:52:33,900 --> 02:52:35,800
Porque si es lo más recomendable quizás no.

1744
02:52:35,960 --> 02:52:40,880
Igual, para este muestro cómo hacerlo, va a ser muy fácil.

1745
02:52:44,940 --> 02:52:50,780
Porque una cosa es hacer toda la explicación de qué es Python, qué es anaconda, cómo intentó hacerle Android.

1746
02:52:50,960 --> 02:53:06,120
Ok, eso es una cosa. Ahora si yo te voy a enseñar a instalar esto, es como aprete un botón y se instala, vas a abrir la terminal y poner dos cosas y se instala y están dando a los 5 minutos. Es muy fácil.

1747
02:53:06,580 --> 02:53:09,840
Claro, no vas a generar mayor tiempo de adaptar.

1748
02:53:09,860 --> 02:53:18,160
No, te vas a generar 10 minutos de tu vida y después vas a tener ya instalado en tu computador y lo vas a abrir y vas a tener otras cositas que son interesantes. Gratis.

1749
02:53:18,859 --> 02:53:19,220
Perfecto.

1750
02:53:19,220 --> 02:53:24,880
por un esfuerzo anula. Mira como decía mi abuelita, el saber no ocupa lugar. Yo se

1751
02:53:24,960 --> 02:53:29,280
haché ahora para que tengo que aprender esto. El saber no ocupa lugar.

1752
02:53:30,620 --> 02:53:36,680
Buenísimo, gracias a propósito. Bueno, con esto terminamos hoy. Así que nada,

1753
02:53:36,820 --> 02:53:42,819
eso, no dejen de practicar. No aflojen, no aflojen para así después llegan los

1754
02:53:42,820 --> 02:53:46,040
mejor preparados posibles a la parte de algoritmos cuánticos. Ok?

1755
02:53:49,301 --> 02:53:50,400
Perfecto, muchas gracias.

1756
02:53:51,680 --> 02:53:53,080
Bueno, gente, nos vemos.

1757
02:53:53,881 --> 02:53:55,260
Que tengan buena semana.

1758
02:53:56,141 --> 02:53:56,900
Buenas semanas.

1759
02:53:57,820 --> 02:54:00,200
Tchau, tchau!


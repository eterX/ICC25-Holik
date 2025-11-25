```
1
00:00:02,400 --> 00:00:03,780
No está bien.

2
00:00:05,720 --> 00:00:10,260
Bueno, ahora tuvimos haciendo unas pruebas ahí, y andaba bien.

3
00:00:13,890 --> 00:00:14,300
Ahí está.

4
00:00:16,980 --> 00:00:17,860
Así que bueno.

5
00:00:18,460 --> 00:00:20,760
Perdona, es pasada un kiram en un momento de esto.

6
00:00:20,770 --> 00:00:23,100
Bueno acá está anunciado ¿ven?

7
00:00:26,000 --> 00:00:35,320
la quinesión del UNAUR, ahora el 28 de noviembre, la Universidad para los estudiantes de UNAUR

8
00:00:36,080 --> 00:00:40,180
pone a disposición micro para transportarse hasta la jornada de fundamento de cuántica,

9
00:00:40,850 --> 00:00:43,660
es un congreso de física cuéntica que nosotros, o sea, sí.

10
00:00:45,000 --> 00:00:54,400
Bueno, este año por cómo son los invites de PICAS, lo más probable es que todo sea en

11
00:00:54,400 --> 00:00:57,140
en el español, acá tienen los charritas invitados,

12
00:00:57,400 --> 00:01:03,880
fue una muy buena oportunidad para enterarse de en qué anda,

13
00:01:04,220 --> 00:01:08,460
la, sí, la física cuántica, la tecnología cuántica,

14
00:01:08,600 --> 00:01:11,360
acá están arriesgando milo, que es de defensa,

15
00:01:11,680 --> 00:01:15,280
desde la parte de investigación del área de defensa,

16
00:01:15,980 --> 00:01:17,620
la TIA-Hampe, desde la CENEA,

17
00:01:18,500 --> 00:01:20,220
eso tiene un laboratorio muy interesante,

18
00:01:20,560 --> 00:01:22,960
ahí en el CENEA yo lo visité, tan bueno.

19
00:01:23,520 --> 00:01:36,300
Bueno, después hay gente, la hora de agartir es de la empresa QuantumSouth, que es una empresa Uwaja,

20
00:01:37,200 --> 00:01:44,360
que el objetivo de esta empresa es resolver problemas de la optimización para cargas de aviones.

21
00:01:45,280 --> 00:01:52,520
Vean que cuando tiene que subir cargas de un avión tienen objetos de distintos pesos y formas.

22
00:01:53,740 --> 00:02:00,460
y distinto valor, entonces tienen que maximizar el valor que llevan teniendo en cuenta la forma y el peso.

23
00:02:01,660 --> 00:02:07,520
Entonces, eso hay una forma de hacerlo con computadoras cuánticos y ellos están en eso,

24
00:02:08,619 --> 00:02:13,840
están tratando de buscar aplicaciones en esa dirección. Así que bueno, ya hay una charlista súper interesante.

25
00:02:14,560 --> 00:02:22,560
quienes quieren venir, ya les digo, para el de una UR, hay micro, la ciudad de Madrid de la facultad

26
00:02:22,860 --> 00:02:29,420
y para quienes no son de una UR, queda en Facultad de Ciencias Exactas y Naturales de la UR, ahí en su

27
00:02:29,480 --> 00:02:37,760
universitaria, están en capital, no es difícil, así que igual es. Bueno, yo voy a empezar entonces con

28
00:02:37,760 --> 00:02:41,220
la clase de UR, ustedes me avisan, ya estamos grabando, sí, perfecto.

29
00:02:47,600 --> 00:02:51,940
Pueden que voy a poner en vez del documento que vamos a ver en su mapa.

30
00:02:58,380 --> 00:02:59,860
Así pongo el pantalla completo.

31
00:03:01,620 --> 00:03:09,460
Bueno, ahí vamos a seguir viendo también coditos de Python para un poco modelar una cosa que

32
00:03:09,460 --> 00:03:16,920
se conoce como el experimento de Max Sander, es un experimento muy conocido, es decir hoy

33
00:03:17,600 --> 00:03:25,660
vamos a empezar viendo repasando cosas de física y para pereciero ustedes para fijar

34
00:03:25,660 --> 00:03:26,580
ideas de

35
00:03:32,420 --> 00:03:33,160
acerca de

36
00:03:38,920 --> 00:03:43,300
qué es la física cuántica porque obviamente como muchos de ustedes no estudiaron física

37
00:03:44,140 --> 00:03:47,640
entonces no sabe mucho cuántica esto va a servir para intentar

38
00:03:49,080 --> 00:03:51,860
a fianzar ideas en el campo.

39
00:03:52,400 --> 00:03:55,960
Bien, y hoy vamos a ver en la segunda parte de la escase

40
00:03:56,720 --> 00:03:58,120
un ejemplo de algoritmo cuántico.

41
00:03:58,300 --> 00:04:02,620
Super sencillo, pero que ilustra la idea de por qué la computación cuántica

42
00:04:03,000 --> 00:04:06,000
podría llegar a tener una ventaja respecto de la computación clásica.

43
00:04:06,320 --> 00:04:07,700
Acaba del ejemplo concreto.

44
00:04:08,880 --> 00:04:10,240
Bueno, empiezo sin más.

45
00:04:11,780 --> 00:04:15,200
Entonces, empezamos viendo un ejemplo de física cuántica,

46
00:04:15,460 --> 00:04:16,859
el interferémetro de la March Center,

47
00:04:17,100 --> 00:04:20,359
vamos a discutir concepto de física y lo vamos a ver en Kisky.

48
00:04:20,700 --> 00:04:26,080
Vamos a aclonar lo que explico con las diapositivas en Kisky.

49
00:04:26,560 --> 00:04:29,800
Después vamos a hacer un pequeño repaso matemática y después

50
00:04:30,060 --> 00:04:33,880
vamos a ver el primer ejemplo de algoritmo cuántico de la materia.

51
00:04:34,220 --> 00:04:36,960
Y a partir de ahora, vamos a ver todo algoritmo cuántico.

52
00:04:37,900 --> 00:04:42,740
Ya estaríamos entrando directamente en el campo de la

53
00:04:42,820 --> 00:04:43,800
computación cuántica.

54
00:04:44,580 --> 00:04:49,480
Lo que pasa es que había que atravesar todo este perípele de matemática y el concepto de física,

55
00:04:50,520 --> 00:04:51,700
porque si no, no se entiende nada.

56
00:04:52,740 --> 00:04:53,560
Pero bueno, ahí está.

57
00:04:54,820 --> 00:04:57,380
Bien, ¿de qué consiste este experimento?

58
00:04:57,940 --> 00:05:03,180
Lo que tienen es un intaxerómetro.

59
00:05:04,360 --> 00:05:07,520
Para ustedes, un intaxerómetro va a ser un dispositivo que tiene,

60
00:05:08,140 --> 00:05:12,720
por el cual entra luz, acá, este input, este rayo negro, es un rayo de luz,

61
00:05:14,020 --> 00:05:18,700
actualmente va a ser luz cuántica, pero en principio piensen que le tiran con un laser

62
00:05:19,860 --> 00:05:27,380
el famoso puntito rojo ilumina con el laser y esto va a pasar primero este

63
00:05:27,440 --> 00:05:35,520
laser va a pasar por un divisor de "as" que acá yo le puse "beam splitter" por la palabra en inglés que es un divisor de "as"

64
00:05:35,940 --> 00:05:41,019
que es un divisor de "as" es un esplejo semilreflectante ustedes conocen este

65
00:05:41,020 --> 00:05:48,340
fenómeno porque cuando van un auto en el colectivo, miran atrás de la ventana y no solo ven lo que hay

66
00:05:48,400 --> 00:05:56,160
afuera, sino que también ven, se ven ustedes mismos a veces, ven que el vidrio en un modo refleja su

67
00:05:56,360 --> 00:06:01,080
carago con un espejo y entonces como puede reflejar y al mismo tiempo ser transparente, igual,

68
00:06:01,220 --> 00:06:06,539
no sé si hay un montón de materiales que son semreflexantes, entonces este divisor de as en

69
00:06:06,540 --> 00:06:17,420
particular lo que va a hacer es dado un rayo de luz entrando, va a reflejar el 50% de la

70
00:06:17,560 --> 00:06:24,720
intensidad de la luz y va a transmitir el otro 50%, cabe a ir a la astrogram.

71
00:06:27,080 --> 00:06:30,100
Entonces, ¿qué hace un espejo semirreflectante?

72
00:06:31,360 --> 00:06:38,220
Cuando entra luz, parte de la luz se transmite y parte de la luz se refleja, ¿sí?

73
00:06:39,040 --> 00:06:45,580
Bien, y acá vamos a poner M1 y acá vamos a poner un M2

74
00:06:48,200 --> 00:06:52,919
y estos van a ser espejos totales, estos reflejan el 100% de la luz, entonces

75
00:06:56,540 --> 00:07:03,600
Los rayos pasan por el primer rayo del uno, pasa por el primer divisor de as, se divide

76
00:07:03,760 --> 00:07:13,540
en dos el rayo y acá se vuelven a juntar los aces y van a ser detectados por estos detectores

77
00:07:13,640 --> 00:07:20,119
que vamos a colocar acá, pero estoy miedo cada espero el pulso, tengo alguna enfermedad

78
00:07:20,120 --> 00:07:23,180
Entonces, va a haber dos versiones del experimento.

79
00:07:25,160 --> 00:07:28,580
Una versión donde no pongo nada en esta zona.

80
00:07:31,000 --> 00:07:36,460
Y otra versión donde sí pongo otro espejo semi reflectante.

81
00:07:36,680 --> 00:07:41,340
Entonces acá va a estar BSE 1, el visor de Asuno y acá va a estar BSE 2.

82
00:07:42,180 --> 00:07:48,199
Fíjense que cuando pongo BSE 2, se haga un kilómetro acá porque este rayo se vuelve

83
00:07:48,200 --> 00:07:54,320
dividir en dos y este otro rayo también se vuelve dividiendo, entonces se junta todo ahí y en

84
00:07:54,420 --> 00:07:58,480
física lo que decimos que va a pasar es que se va a producir un fenómeno de interferencia.

85
00:08:00,879 --> 00:08:16,959
Buena, se entiende este dibujo, entonces tenemos el input que es luz, va al unividor de

86
00:08:16,960 --> 00:08:20,260
la luz se divide en dos y sigue su camino.

87
00:08:24,380 --> 00:08:26,520
Los rayos de luz se vuelven a juntar acá,

88
00:08:27,480 --> 00:08:29,960
si no hay nada, pasan así como si nada

89
00:08:30,860 --> 00:08:33,180
a unos detectores que vamos a llamar de seres de uno,

90
00:08:33,479 --> 00:08:34,700
detectores de luz en principio.

91
00:08:36,300 --> 00:08:39,900
Y si hay algo también, pero si ponemos el segundo divisor de das,

92
00:08:40,440 --> 00:08:42,659
va a haber una nueva reflexión y transmisión

93
00:08:42,800 --> 00:08:44,720
de este rollo de abajo y el largo rollo de arriba.

94
00:08:45,520 --> 00:08:50,260
al brazo de arriba del interferómetro le llamamos modo 1 y el brazo de abajo modo 0

95
00:08:51,360 --> 00:08:55,700
M1 y M2 son espejos 100% reflectantes

96
00:08:56,980 --> 00:09:02,960
Y BC1 y BC2 son divisores de AS o semi-espejos

97
00:09:03,410 --> 00:09:09,959
que tienen la propiedad de transmitir el 50% de la luz inciente y reflejar el 50% de la luz inciente

98
00:09:09,960 --> 00:09:14,960
Y acá hay otro elemento que le pusimos PS por FaceShifter,

99
00:09:15,280 --> 00:09:16,420
vamos, cambia de fases.

100
00:09:16,600 --> 00:09:21,960
Este cosito lo que hace es cambiar la fase de la luz que entra por esto.

101
00:09:22,520 --> 00:09:30,180
Para que no venga de física, cambiar la fase puede ser equivalente a hacer circular el rayo de luz por un medio que no sea aire.

102
00:09:30,420 --> 00:09:40,780
por ejemplo, si el rayo de abajo va todo por aire y al de arriba pone agua o pone algún tipo de líquido

103
00:09:41,780 --> 00:09:49,520
cuyo índice de reflexión depende de la temperatura y que esa temperatura se pueda juntar controlando una corriente eléctrica

104
00:09:50,300 --> 00:09:59,499
en el carismo que fuere que permita agregarle una diferencia de caminos de fase a el brazo de arriba y el brazo de abajo

105
00:10:00,480 --> 00:10:02,520
¿Preguntas acerca del setup experimental?

106
00:10:06,600 --> 00:10:07,700
Por momento ninguno.

107
00:10:09,100 --> 00:10:10,520
Por momento ninguno, perfecto.

108
00:10:11,480 --> 00:10:17,760
Bien, ahora obviamente a nosotros lo que nos interesa es que va a pasar en el caso cuántico.

109
00:10:20,320 --> 00:10:26,020
Volvamos a la pizarra, en el caso cuántico, en vez de tirar un rayo de luz.

110
00:10:29,440 --> 00:10:35,040
Si tiraba un rayo tenía 50% reflejado, 50% transmitido.

111
00:10:35,940 --> 00:10:43,300
Si ahora tiro, lo hago al LASER, entrar en un régimen cuántico en el cual voy tirando fotones de A1,

112
00:10:43,600 --> 00:10:44,780
supongo que este era el LASER, ¿no?

113
00:10:47,220 --> 00:10:53,620
Supongo que el LASER tiene mucha coherencia y que le atenuamos la intensidad de forma tal de que los fotones van saliendo de A1.

114
00:10:53,620 --> 00:11:01,880
Bueno, lo que va a pasar, si yo pusiera detectores acá y acá, es que a veces voy a detectar

115
00:11:01,880 --> 00:11:07,600
un fotón acá arriba que corresponde a que el fotón Chocóis se reflejo y a veces un

116
00:11:07,640 --> 00:11:14,180
fotón abajo que corresponde a que el fotón se transmitió. Fíjense que si acá arriba

117
00:11:14,380 --> 00:11:23,600
ponía detectores de 1 y 2, entonces acá voy a tener el 50% de la luz y acá voy a tener

118
00:11:23,600 --> 00:11:32,360
de la luz. Eso con luz clásica, con la luz de un puntero láser si quieren. Pero si el láser

119
00:11:33,260 --> 00:11:40,020
fuera atenuado y preparado de forma tal de que tiran fotones de uno, bueno, la mitad de los fotones

120
00:11:40,700 --> 00:11:48,260
irían para arriba y la mitad de los fotones se reflejarían y la mitad se transmitirían,

121
00:11:48,260 --> 00:11:55,160
¿Ok? Se entiende la diferencia de comportamiento entre la luz clásica y la luz cuántica.

122
00:11:55,680 --> 00:11:59,600
En el caso cuántico que estamos discutiendo acá, atención.

123
00:12:01,760 --> 00:12:07,320
Hay comportamientos cuánticos de la luz más generales, pero acá vamos a discutir el comportamiento discreto.

124
00:12:08,080 --> 00:12:13,280
Estamos imaginando que tenemos una fuente de luz que tira fotones aún.

125
00:12:14,440 --> 00:12:18,540
y fenomenicamente lo que se observa es que la mitad se transmite de las

126
00:12:18,660 --> 00:12:26,200
fotones y la metas se refleja. Si tiraran 100 fotones esto sería como una

127
00:12:26,260 --> 00:12:29,160
moneda. Veo que hay gente ahí preguntando.

128
00:12:30,120 --> 00:12:33,940
Si yo tengo una pregunta. Un naz de luz está compuesto por fotones.

129
00:12:34,640 --> 00:12:40,180
Cómo sería esa parte? Sí más o menos, más o menos porque es súper complejo el tema de

130
00:12:40,180 --> 00:12:48,760
porque claro obviamente cuando vas a estudiar un poco de física te dicen que las partículas

131
00:12:48,880 --> 00:12:56,820
elementales de la luz son las fotos, usted dice si tienes un átomo o una molécula de que están

132
00:12:56,900 --> 00:13:02,540
hechas las moléculas, bueno de átomos y los átomos están hechos de protones, neutrones,

133
00:13:02,620 --> 00:13:10,780
electrones y cuando te dices bueno cuando tenés luz la luz está echada el fotón, no

134
00:13:10,800 --> 00:13:15,740
cuál es parcialmente cierto, pero es parcialmente cierto porque si bien vos

135
00:13:15,820 --> 00:13:22,040
podés preparar a la luz en un estado cuántico y observar el carácter si querés

136
00:13:22,180 --> 00:13:26,620
individual de los fotones por ejemplo por tener una fuente que como te decía antes

137
00:13:26,620 --> 00:13:34,420
vaya tirando fotones de uno y qué significa eso, atención, vamos a hacer unos dibujos.

138
00:13:35,500 --> 00:13:40,120
Cuando decís analizar la luz a nivel cuántico sería llegar a ver los fotones,

139
00:13:41,420 --> 00:13:56,600
no detener al final y ir a los fotones. Es más complejo que eso pero sí, no, no, no, no, no, no, no, no, no, no, no, no, no, no, no, no

140
00:13:57,740 --> 00:14:06,140
lo que verías suposete que tu detector produce como resultado la interacción de la luz con la

141
00:14:06,180 --> 00:14:10,760
materia una corriente entonces cuando te ves el laser apagado vos verías que hay una corriente

142
00:14:11,780 --> 00:14:17,200
nula y de repente cuando prendes el laser aparece un nivel de corriente ¿entendés?

143
00:14:20,660 --> 00:14:24,540
bien y después cuando volvés a apagar el laser esto se apagaría

144
00:14:25,060 --> 00:14:26,760
verías una cosa más o menos así

145
00:14:30,660 --> 00:14:32,820
un modelo sencillo de la luz

146
00:14:33,520 --> 00:14:37,180
vos podrás pensar a la luz como un montón de micro pelotitas

147
00:14:38,220 --> 00:14:39,520
que lo han agido como entendés

148
00:14:41,040 --> 00:14:43,580
que serían los fotones, no son pelotitas, no importa

149
00:14:43,920 --> 00:14:45,100
pensálo por un minuto así

150
00:14:45,560 --> 00:14:47,620
entonces ahí vos verías una cosa así, qué dirías?

151
00:14:47,740 --> 00:14:52,540
cada fotoncito, me genera un pulcito de corriente y si tiro muchos

152
00:14:53,120 --> 00:15:12,560
esto es proporcional a la cantidad de fotones que impactan por unidad de tiempo. Ahora, vos suponente que podés atenuar la intensidad de la fuente de forma tal de que tiene tan baja intensidad que el número de fotos es muy bajo y es tan bajo que tira un fotón por segundo.

153
00:15:13,199 --> 00:15:28,060
en serie, claro en serie tipo trencitos de fotones, claro entonces vos por ahí no ves nada y de repente ves un cosito así y de repente ves duplicado esto, ¿entendés? o triplicado ¿entendés? ¿me entendés?

154
00:15:29,440 --> 00:15:33,740
ahí que acá hay un fotón acá entran dos fotones acá tres fotones, estoy haciendo

155
00:15:33,820 --> 00:15:38,740
medio, pero esto es más o menos así, esto es más o menos así, vos puedes preparar la

156
00:15:38,900 --> 00:15:45,540
fuente laser de forma tal de que tenés cero corriente y de repente un pulcito y ese pulcito

157
00:15:45,620 --> 00:15:54,120
corresponde a la llegada de un fotón, bueno, ¿por qué esto es así? porque hay materiales

158
00:15:54,120 --> 00:15:57,440
que tiene la capacidad de que cuando le pegue un fotón,

159
00:15:58,780 --> 00:16:00,120
genera una corriente eléctrica.

160
00:16:00,240 --> 00:16:01,880
¿Por qué? Porque la idea sería que

161
00:16:02,360 --> 00:16:05,300
tan los electrones hay en el material que yo en un átomo,

162
00:16:07,740 --> 00:16:11,460
y cuando le pega luz, el electrón se excita y

163
00:16:13,160 --> 00:16:16,440
si el material está construido de una manera peculiar,

164
00:16:16,760 --> 00:16:21,920
vos podés lograr que esa energía que le da el fotón al electrón que se excita

165
00:16:22,120 --> 00:16:30,240
se transforme en una corriente porque se amplifica. Lo cual sería un foto multiplicador básicamente.

166
00:16:32,660 --> 00:16:39,240
Bien, certiendo un poco la idea, entonces acá estaríamos imaginando que podamos tirar

167
00:16:39,360 --> 00:16:43,800
fotones de la uva. Por la duda se aclaró la situación es bastante más compleja.

168
00:17:13,839 --> 00:17:19,400
de uno y de dos son eventos individuales, entonces los que se reflejan, pum, ve un pulso

169
00:17:19,560 --> 00:17:22,860
acá arriba y los que se transmiten ve un pulso acá abajo.

170
00:17:23,980 --> 00:17:29,480
Ok, o sea más que todo, tú estás explicando de una manera implícita es el experimento

171
00:17:29,520 --> 00:17:33,000
este del fotoelectrón, de Einstein creo que es.

172
00:17:33,140 --> 00:17:39,260
Claro, el efecto fotoeléctrico, básicamente si vos podrías armar un detector en base

173
00:17:39,840 --> 00:17:41,620
tomando como va a ser efecto fotoeléctrico.

174
00:17:43,440 --> 00:17:51,820
ok, ok bien, básicamente el pulso representa como que el electromagnetismo ahí se hace

175
00:17:51,840 --> 00:17:59,420
enmide por medio de eso. Claro que el que el que el fotón lleva una energía, un paquetito

176
00:17:59,420 --> 00:18:06,240
de energía que permite disparar una cascada de electrones que vos puedes amplificar y ver

177
00:18:06,240 --> 00:18:15,300
bueno, no puedo ver un fotón, bueno, lo que puede ver es el efecto del fotón que lleva

178
00:18:15,380 --> 00:18:20,840
energía y que por endel produjo una corriente, ¿entendés?

179
00:18:21,800 --> 00:18:27,480
Y la corriente de oscila puedes medir con un aparatomacroscópico, ¿entendés?

180
00:18:28,340 --> 00:18:36,220
Entonces acá la idea sería, pero la realidad es así, es mucho más complejo porque uno

181
00:18:36,220 --> 00:18:42,820
diría "bueno, la luz es estrecha de fotones, tengo un laser y que es un rayo de luz" y bueno,

182
00:18:42,960 --> 00:18:50,680
muchos fotoncitos tipo que son como pelotitas que viajan y si uno mira un poco como son las cosas

183
00:18:50,780 --> 00:18:55,120
pareciera que es así, pero no es así en realidad porque en la descripción cuántica de la luz,

184
00:18:55,740 --> 00:19:01,220
cuando, típicamente cuando uno produce un estado cuántico del campo electronomandrético tiene

185
00:19:01,220 --> 00:19:18,800
una superposición así, vamos a poner sí, alfa y por y, una cosa de este tipo, alfa

186
00:19:19,380 --> 00:19:29,080
cero por cero más alfa uno por uno, más alfa dos por dos, ahora explico que es esto,

187
00:19:29,180 --> 00:19:32,220
Bueno, esto sería un estado con cero fotones.

188
00:19:32,870 --> 00:19:35,620
Es decir, el ground state del campo electromagnético.

189
00:19:36,120 --> 00:19:37,180
Campo no excitado.

190
00:19:37,790 --> 00:19:39,540
Pero este estado no tiene fotones.

191
00:19:40,340 --> 00:19:42,780
Después, con una cierta probabilidad,

192
00:19:43,840 --> 00:19:44,840
tendrías un fotón.

193
00:19:45,080 --> 00:19:46,740
Con otra cierta probabilidad, dos fotones.

194
00:19:46,940 --> 00:19:48,320
Con otra cierta probabilidad, tres fotones.

195
00:19:48,500 --> 00:19:48,600
Así.

196
00:19:48,980 --> 00:19:51,380
Y en real son así los estados cuánticos generales.

197
00:19:52,640 --> 00:19:54,460
Bueno, no todo, algunos son así.

198
00:19:54,710 --> 00:19:55,560
Estoy poniendo un ejemplo.

199
00:19:56,700 --> 00:20:01,720
la peculiaridad de este estado es que es una superposición, es como un gato de

200
00:20:01,900 --> 00:20:05,220
Schrodinger, con distintos números de partículas.

201
00:20:06,380 --> 00:20:12,920
Entonces, este estado del campo electromagnético no se puede pensar como un

202
00:20:13,100 --> 00:20:16,080
chorro de fotones porque no tiene número de fotones definidos.

203
00:20:18,380 --> 00:20:23,640
Entonces, vos en el laboratorio cuando armes un estado de un fotón vas a hacer algo así,

204
00:20:23,660 --> 00:20:34,540
alfa 0 por 0 más alfa 1 por 1, donde alfa 0 al cuadrado más alfa 1 al cuadrado es solo la 1,

205
00:20:37,000 --> 00:20:43,620
entonces este estado con una probabilidad no despeciable tira un fotón, pero típicamente

206
00:20:43,800 --> 00:20:48,500
bueno te puedes sacar de encima estos otros términos que son el tipo alfa 2 por 2 fotobuses,

207
00:20:48,780 --> 00:20:55,000
pero tienen una probabilidad mucho menor. Es decir, en física se hacen muchas idealizaciones,

208
00:20:56,140 --> 00:21:05,880
pero la idea es que, sí, que bueno, el "bog boss" al final del día no es un buen

209
00:21:06,100 --> 00:21:13,140
picture pensar a la luz como un rayo de fotones, como si fuera un chorro de fotones, es algo más complejo.

210
00:21:14,700 --> 00:21:20,580
Desde el punto de vista moderno o contemporáneo, un físico de randa cualquiera va a pensar

211
00:21:20,700 --> 00:21:29,800
la luz como un campo que eventualmente en cierta escala se comporta cuánticamente y

212
00:21:29,960 --> 00:21:35,160
que los fotones serían excitaciones fundamentales del campo.

213
00:21:35,300 --> 00:21:40,239
En este caso el campo es el campo electromagnético y ahí se termina medio el historia porque

214
00:21:41,640 --> 00:21:47,660
es como uno ya se empieza a familiarizar con los campos cuánticos, chau. Pero con esto no quiero

215
00:21:47,820 --> 00:21:54,760
decir que te esté dando de esa forma un picture corrente, viste, dice yo. Matemáticamente funciona,

216
00:21:55,120 --> 00:22:00,520
pero bueno, hay muchos programas filosóficos asociados a entender que es la luz, que es un

217
00:22:00,520 --> 00:22:07,020
campo cuantio pero bueno lo que nos importa a nosotros es que efectivamente

218
00:22:07,520 --> 00:22:14,640
efectivamente si yo hago el setup experimental y pongo el primer mid-blitter

219
00:22:16,240 --> 00:22:25,020
los espejos M1 y M2, el safe shifter por acá y pongo de vuelta el coso

220
00:22:25,040 --> 00:22:33,960
está acá y los detectores, lo que va a ver pasando es que si tiran luz pasa lo que puse

221
00:22:33,960 --> 00:22:39,080
en las diapositivas, ahora si tiran fotones de A1 podrían tener una situación en la

222
00:22:39,160 --> 00:22:47,860
cual el fotón se refleja en el primer divisor de A, se refleja en este espejo, pasa por el

223
00:22:47,880 --> 00:22:53,520
cambiador de cosas y acá tiene que volver a elegir, o se refleja o se está bien, o podría

224
00:22:54,480 --> 00:23:05,500
una posibilidad para un fotón es esta, es un camino posible, un fotón podría haber hecho eso, ahora

225
00:23:05,700 --> 00:23:14,160
repito el experimento, por el otro fotón hace esto, ay que tonto, está mal dibujado, perdón,

226
00:23:14,720 --> 00:23:17,440
como que me quedó este espejo de acá, ven

227
00:23:23,400 --> 00:23:26,280
yo tengo que dibujar un poco más acá, así, bien

228
00:23:28,940 --> 00:23:30,180
otro fotón puede hacer esto

229
00:23:31,080 --> 00:23:34,800
se transmite acá, se refleja acá y acá se vuelve a transmitir

230
00:23:35,000 --> 00:23:36,060
es otro camino posible

231
00:23:36,440 --> 00:23:44,180
o podría haber hecho en vez de eso, podría haber hecho esto, esto, esto, esto

232
00:23:44,180 --> 00:23:53,420
De hecho, en cada experimento hay una, dos, tres, cuatro, cinco...

233
00:23:53,820 --> 00:23:54,300
No, dos.

234
00:23:55,290 --> 00:23:57,200
No, hay cuatro posibilidades, ¿sí?

235
00:23:58,120 --> 00:24:01,880
Porque el fotón se encuentra con dos alternativas acá,

236
00:24:02,760 --> 00:24:05,680
hay dos historias posibles para el fotón, hay dos caminos acá,

237
00:24:05,880 --> 00:24:07,240
o sea, refleja se transmite,

238
00:24:07,890 --> 00:24:13,420
y después cuando se vuelve a encontrar acá, se encuentra con dos posibilidades más.

239
00:24:13,540 --> 00:24:19,960
Entonces al final hay 2 a la 2 posibilidad, que es 2 a la 4, 2 a la 2 que es 4, ok? 4 posibilidad.

240
00:24:20,280 --> 00:24:20,980
¿Se entiende esto?

241
00:24:24,200 --> 00:24:24,340
Sí.

242
00:24:24,640 --> 00:24:25,260
Bien.

243
00:24:25,820 --> 00:24:25,900
Sí.

244
00:24:27,580 --> 00:24:28,060
Bien.

245
00:24:29,060 --> 00:24:33,640
Bueno, eso es en lo relativo al setup experimental.

246
00:24:33,900 --> 00:24:41,140
Y hay 2 experimentos que son distintos, porque pongo el segundo divisor de AS o no lo pongo, ok?

247
00:24:41,940 --> 00:24:45,900
no se puede poner y no poner un divisor de A, o lo ponen o no lo ponen.

248
00:24:46,290 --> 00:24:51,440
Si lo ponen es un cierto contexto de experimentación y si no lo ponen es otro contexto de experimentación.

249
00:24:52,120 --> 00:24:54,080
Es parecido a la doble rendija, ¿se acuerdan?

250
00:24:55,180 --> 00:25:02,300
Cuando discutíamos la doble rendija que yo podía elegir, o poner los aparatos para medir por qué la rendija pasó, o no ponernos.

251
00:25:02,410 --> 00:25:03,140
Pues acá es lo mismo.

252
00:25:04,000 --> 00:25:06,000
O pongo el segundo divisor de A o no.

253
00:25:07,740 --> 00:25:07,900
Bien.

254
00:25:08,740 --> 00:25:10,220
A y vuelvo, vuelvo acá, ¿no?

255
00:25:10,640 --> 00:25:13,580
Déjenme hacer un dibujo mejor porque es importante esto.

256
00:25:16,740 --> 00:25:22,980
¿El FaceShifter es como que polariza el otro vaso de luz de forma distinta?

257
00:25:23,940 --> 00:25:33,660
No, lo que te hace es el FaceShifter es para que dibujo cada uno de los vasos.

258
00:25:35,640 --> 00:25:41,860
Lo que está haciendo este bichito es que te cambia la longitud de camino óptico del

259
00:25:42,000 --> 00:25:56,280
foto. Si tuviera que explicar el camino óptico me llevaría bastante tiempo, pero pensalo

260
00:25:56,340 --> 00:26:02,299
como que metés un medio diferente en un mes y eso hace que matemáticamente se le

261
00:26:02,300 --> 00:26:13,140
le agrego una fase al estado cuántico. Bien. Entonces lo que va a ir pasando es que yo

262
00:26:13,140 --> 00:26:22,280
tiro un fotón, tiro uno y entonces podría pasar que se transmite acá y se transmite

263
00:26:22,280 --> 00:26:27,060
de vuelta entonces lo detecto acá, entonces tengo una cuenta acá o podría darse reflejada,

264
00:26:27,060 --> 00:26:33,220
en una cuenta acá y así entonces yo lo que voy a ver fenoménicamente se entiende

265
00:26:33,780 --> 00:26:41,440
fenoménicamente es que los detectores de uno y de dos van a ir clicando porque a

266
00:26:41,520 --> 00:26:44,680
veces cada un fotón acá arriba y a veces cada acá abajo

267
00:26:46,020 --> 00:26:51,380
había cuatro posibilidades todos esas posibilidades terminan con un fotón en

268
00:26:51,380 --> 00:26:57,540
de uno y dos de esas posibilidades terminan con un foto de en de dos, entonces en una tirada tengo

269
00:26:58,120 --> 00:27:03,060
en de uno, en otro en de dos, en otro tengo en de uno, ¿se entienden?

270
00:27:05,200 --> 00:27:05,600
Sí

271
00:27:07,680 --> 00:27:12,820
Por ahí repite, por ahí en tres tiradas repítican en tres en de uno, yo voy tirando muchos

272
00:27:13,080 --> 00:27:14,740
fotones, todos en el mismo estado, ¿sí?

273
00:27:16,620 --> 00:27:23,920
Y es como una moneda, se envuelta al final del día, si los espejos son 50 y 50 es como

274
00:27:23,940 --> 00:27:31,300
una moneda, pero vamos a ver después que el phase shifter hace quilombito y va a alterar

275
00:27:31,300 --> 00:27:37,620
las probabilidades de esta moneda, esa es la idea, va a producir lo que se conoce como

276
00:27:37,620 --> 00:27:44,000
un fenómeno de interferencia, fíjense otra cosa que puede estar buena de discutirla ahora,

277
00:27:44,860 --> 00:27:56,440
yo no pongo, esperen que si puedo, vamos a sacar al segundo divisor de as, pero es más fácil

278
00:27:56,520 --> 00:28:03,640
pensarlo así ¿no? que pasa si saco al segundo divisor de as, pongo el face shifter, bien,

279
00:28:04,880 --> 00:28:12,239
tira un fotón o se transmite y se refleja en dedos y cae en el detector de arriba o

280
00:28:12,240 --> 00:28:15,360
o se refleja y cae el detector de abajo.

281
00:28:15,820 --> 00:28:17,300
Hay sólo dos posibilidades.

282
00:28:17,590 --> 00:28:21,540
Si no pongo el segundo divisor de AS,

283
00:28:21,780 --> 00:28:23,900
sólo tengo dos posibilidades para los fotones.

284
00:28:25,420 --> 00:28:29,560
Lo que va a pasar es que, en ese caso,

285
00:28:31,220 --> 00:28:34,160
no va a importar la fase que yo le meto acá en PS.

286
00:28:35,280 --> 00:28:38,359
Como que el resultado experimentario

287
00:28:38,440 --> 00:28:41,860
va a ser insensible a la fase que le pongo.

288
00:28:43,240 --> 00:28:46,100
Pero lo que me importa que se entienda es la fenomenología.

289
00:28:46,320 --> 00:28:49,920
¿Por qué? Bueno, porque este experimento se puede hacer

290
00:28:50,640 --> 00:28:53,500
en el laboratorio, de hecho, en Argentina se hace eso.

291
00:28:54,160 --> 00:28:56,260
Se podría hacer una base cotidiana.

292
00:28:57,060 --> 00:29:01,340
Hoy por hoy es un experimento sencillo, no tiene mucha magia.

293
00:29:02,900 --> 00:29:04,180
Sí, obviamente hay que sabar, no?

294
00:29:04,240 --> 00:29:07,680
Pero dentro de todo no es un experimento sofisticado.

295
00:29:07,840 --> 00:29:10,900
los laboratorios de óptica cuántica argentina,

296
00:29:11,160 --> 00:29:13,160
de Argentina típicamente pueden hacer esto.

297
00:29:14,540 --> 00:29:15,980
Entonces esto es lo que pasa realmente.

298
00:29:16,400 --> 00:29:20,860
Ustedes detectan en los detectores el carácter discreto de la luz.

299
00:29:21,820 --> 00:29:24,880
Y esto va a una computadora, a una PC.

300
00:29:25,600 --> 00:29:26,700
¿Qué hace la computadora?

301
00:29:26,780 --> 00:29:29,200
Va guardando los resultados de los detectores.

302
00:29:31,620 --> 00:29:33,900
Y de esa forma ustedes pueden calcular probabilidades.

303
00:29:34,080 --> 00:29:36,799
Probabilidad de que sea detectado el fotón

304
00:29:36,800 --> 00:29:41,540
en el detector de arriba, probabilidad de que sea detectada el fotón en el detector de abajo, ¿sabes?

305
00:29:44,160 --> 00:29:46,320
Como que es importante entender la fenomenología.

306
00:29:47,680 --> 00:29:55,780
¿Por qué? Bueno, porque esto ocurre realmente, o al menos este fenómeno es lo que más o menos se observa en laboratorio.

307
00:29:56,280 --> 00:30:05,799
Las cosas obviamente son mucho más complejas porque lo que uno va a detectar en los detectores es por ahí una corriente de base

308
00:30:05,800 --> 00:30:10,040
que tiene que ver con el rube ambiente y uno la tiene que restar y ahí recién ve los piquitos,

309
00:30:10,200 --> 00:30:16,820
los punicitos que corresponden a cada fotón y también la otra cosa que puede pasar es que la

310
00:30:16,860 --> 00:30:23,100
fuente cada tanto tira en vez de un fotón que con una cierta probabilidad de error tira dos fotones

311
00:30:23,180 --> 00:30:28,660
o tres o cuatro, entonces ahí lo que observa de los detectores es más complejo. Sin embargo,

312
00:30:29,080 --> 00:30:35,780
uno puede setear las cosas como para que la realidad se comporte más o menos así y preparar

313
00:30:35,780 --> 00:30:44,720
este tipo de interferometría tiene incluso aplicaciones tecnológicas no vamos a mencionar

314
00:30:44,920 --> 00:30:50,580
ahora vamos a hablar más adelante sobre ellas pero pero la idea es que esto es algo que les

315
00:30:50,640 --> 00:30:56,500
debería hacerle a ustedes para fijar ideas acerca de qué es un fenómeno cuántico básicamente

316
00:30:56,700 --> 00:31:12,640
si ustedes van a un laboratorio, no, de algún laboratorio real, bueno, que se llama.

317
00:31:14,720 --> 00:31:17,640
Si van laboratorios por ahí van a ver algo así, como esto de acá.

318
00:31:25,280 --> 00:31:25,440
no

319
00:31:32,900 --> 00:31:37,040
a casa se lo pueden comprar también, bueno, pero ven que ahí están

320
00:31:40,440 --> 00:31:48,260
los divisores de A, los fake shift, básicamente se van a un laboratorio para ver una mesa óptica

321
00:31:48,810 --> 00:31:52,740
y en la mesa óptica van a estar los instrumentos ópticos, espejos,

322
00:31:53,360 --> 00:31:57,920
espejos semi reflectores, cambiadores de fase, polarizadores, lo que se ve, así.

323
00:31:58,880 --> 00:32:05,880
y ustedes a nivel cuántico no van a ver nada, lo único que van a ver es las cuentas que aparecen

324
00:32:05,880 --> 00:32:17,480
en la computadora, de aquí de acá, lo único que van a recibir como salida el experimento es lo que

325
00:32:17,620 --> 00:32:23,139
cuenta, lo que registra la computadora, no es que van a ir a cuando lo corran pero probablemente no

326
00:32:23,140 --> 00:32:28,860
no hay nada, porque tampoco es que va a lavar el rayo, ni el camino, ni nada, porque el ojo

327
00:32:29,480 --> 00:32:41,300
no detecta fotones de alguna. Entonces, bueno, se entiende eso más o menos, todo esto era

328
00:32:41,400 --> 00:32:45,700
para que un poco fíjene de qué hace, cómo sería un ejemplo de sistema cuántico, uno

329
00:32:45,780 --> 00:32:51,660
al mes, para que tenga la idea. Y este ejemplo es lo suficientemente sencillo como para que

330
00:32:51,660 --> 00:32:57,380
hagamos las cuentas, ¿puedes hacer las cuentas? ¿Cómo funciona esto?

331
00:32:59,440 --> 00:33:07,300
Bien, entonces al brazo de abajo que se dio el modo 0, lo vamos a representar con el ket

332
00:33:07,620 --> 00:33:16,120
0, ¿sí? Como una computadora cuántica con este el 0 de la base computacional y al brazo

333
00:33:16,120 --> 00:33:22,040
arriba al modo 1 lo representamos con el ket 1, ¿qué quiere decir esto?

334
00:33:22,280 --> 00:33:29,080
bueno que si un fotón está físicamente localizado en este brazo

335
00:33:30,440 --> 00:33:34,200
entonces ese va a ser el ket 0 y lo mismo para el ket 1

336
00:33:42,120 --> 00:33:48,980
y a la larga ya pueden ir viendo que este fotón que está ahí viajando en los teléfono de Mach-Celner

337
00:33:49,180 --> 00:33:52,960
es como un qubit, porque es un sistema de dimensión 2, hay dos modos

338
00:33:53,880 --> 00:33:58,400
dos modos y dos detectores, dos posibilidades de detectar, de ser de un...

339
00:33:59,640 --> 00:33:59,920
verlo

340
00:34:01,640 --> 00:34:07,120
bueno, y los divisores de AS se pueden representar por las siguientes matrices

341
00:34:07,120 --> 00:34:14,800
quiere decir esto que el efecto que le hace al estado del fotón atravesar el

342
00:34:14,940 --> 00:34:20,260
beamplitter se puede describir matemáticamente por la multiplicación

343
00:34:21,560 --> 00:34:29,120
por esta matriz, esa es la idea y el efecto el phase shifter se puede, si

344
00:34:29,159 --> 00:34:35,040
sabemos cuando el fotón atraviesa el phase shifter, el efecto se representa con

345
00:34:35,040 --> 00:34:37,540
la multiplicación por esta otra matriz, ¿está bien?

346
00:34:42,159 --> 00:34:49,360
Entonces bueno, acá volvemos, el fotón entra a la salida del primer...

347
00:34:51,040 --> 00:34:57,080
En la entrada hasta en el modo 0, a la salida del primer divisor de AS,

348
00:34:58,740 --> 00:35:01,020
tenemos que multiplicar a 0 por esta matriz.

349
00:35:01,840 --> 00:35:06,740
entonces tengo que hacer "bc1" por cero, me queda "c1"

350
00:35:08,520 --> 00:35:13,240
ahora cuenta como ejercicio, ustedes tienen que hacer todo esto en sus casas

351
00:35:14,920 --> 00:35:20,480
les queda esto de acá y esto es parecido a un vector que ya habíamos analizado en clase

352
00:35:21,080 --> 00:35:26,500
que era el más, pero la verdad no tiene el más, sino que tiene el más con una fase "i"

353
00:35:33,020 --> 00:35:44,120
Bien, entonces esto es el estado del sistema cuántico a la salida del primer divisor de

354
00:35:44,220 --> 00:35:53,060
AS, ahora el otro sistema con el cual se encuentra nuestro fotón es el cambiador de

355
00:35:53,060 --> 00:36:00,420
de fases, el "FakeShifter", entonces al "Psi1" del paso anterior lo multiplicó por "ps",

356
00:36:00,500 --> 00:36:05,940
pues agarro el estado del caso anterior lo multiplicó por "ps", me queda esto de acá

357
00:36:10,440 --> 00:36:18,120
y por último, por último analicemos primero la situación en la cual pongo un segundo "BinSplitter"

358
00:36:21,260 --> 00:36:27,340
al estado del paso anterior lo multiplico por bs2, entonces tengo esto por esto, ok?

359
00:36:28,190 --> 00:36:33,740
voy a hacer un diagrama esquemático de esto en la pizarra

360
00:36:39,299 --> 00:36:43,400
como se vería esto? bueno, yo empiezo con cero, ok?

361
00:36:45,260 --> 00:37:04,880
la aplico el primer bs, bs1, me queda bs1 por 0, ahora la aplico bs, entonces me queda bs por bs1 por 0

362
00:37:07,260 --> 00:37:23,960
y ahora le aplico bs2 y me queda bs2 por bs1 por c, ¿a que se parece esto?

363
00:37:29,260 --> 00:37:39,480
a una diagonalización. No, no quiero leerlo. Bueno, poco así se parece, pero no es un circuito cuántico.

364
00:37:40,360 --> 00:37:54,360
Piénsenlo así, tengo el 0 y tengo Bs1, tengo PS, ¿entendés? y tengo Bs2, ahora y acá mío,

365
00:37:55,380 --> 00:37:56,920
no se parece un circuito?

366
00:37:59,640 --> 00:38:00,160
si

367
00:38:01,280 --> 00:38:02,000
es un circuito

368
00:38:03,100 --> 00:38:06,500
porque en cada paso yo estoy multiplicando por matrices unitarias que son

369
00:38:06,660 --> 00:38:08,800
ps1, ps2

370
00:38:10,900 --> 00:38:11,420
bueno

371
00:38:11,570 --> 00:38:12,320
y efectivamente

372
00:38:12,610 --> 00:38:13,860
esto se puede hacer con circuitos

373
00:38:13,990 --> 00:38:15,120
voy a hacerlo con quisky

374
00:38:16,440 --> 00:38:17,440
importamos cositas

375
00:38:19,080 --> 00:38:20,520
yo después les paso el canal de buco

376
00:38:23,260 --> 00:38:23,500
entonces

377
00:38:23,860 --> 00:38:25,240
acá el circuito es muy sencillo

378
00:38:25,240 --> 00:38:25,360
cuando se va a hacer un circuito

379
00:38:25,360 --> 00:38:33,900
tiene un solo Q8 que sería nuestro fotón, algo un quantum circuit con un fotón, ok?

380
00:38:34,470 --> 00:38:43,580
de este circuito lo llamé mc, el mach sender. Luego define la matriz de esto, vamos a hacer así.

381
00:38:44,920 --> 00:38:46,940
Fíjense que acá usted no pique.

382
00:39:02,920 --> 00:39:08,240
ven que acá definí la matriz está acá

383
00:39:13,200 --> 00:39:19,920
la bs1 que es igual a bc2, 1/2 por 1i i1

384
00:39:21,780 --> 00:39:26,160
esta la definí así, fíjese que lo tengo escrito acá arriba,

385
00:39:26,500 --> 00:39:31,280
vamos a ver si, me voy a tratar de aislar las funciones identificadas

386
00:39:32,960 --> 00:39:40,380
esto es npri, que lo que hace es lo que venga acá dentro, como puntitos

387
00:39:41,080 --> 00:39:49,180
acabo de definir un objeto que es una raid en un P, para nosotros va a ser una matriz

388
00:39:51,440 --> 00:39:58,600
luego la matriz, ¿cómo la definimos? primero armo un primer corchete y lo cierro con este

389
00:39:58,660 --> 00:40:03,560
corchete y acabo de poner la primera fila

390
00:40:05,480 --> 00:40:13,820
coma la segunda fila en general como sería definir una matriz m sería np punto

391
00:40:13,820 --> 00:40:21,320
de array, abre paréntesis, abre y cierro corchete y acabo de poniendo las filas

392
00:40:22,540 --> 00:40:31,500
fila 1, fila 2, fila 1, se entiende?

393
00:40:34,240 --> 00:40:38,360
bueno si tuviera que poner números concretos tendría que poner que yo 1 2 3

394
00:40:40,740 --> 00:40:52,520
4 5 6, vamos a hacer una de 3 por 3, 7 8 9

395
00:40:59,580 --> 00:41:08,240
no hace falta que ordenen las cosas, eso lo hago porque estoy en falta, o sea, bien, ahí,

396
00:41:08,930 --> 00:41:14,980
por qué acá no me dejo escribir M, ahí, ven que si primero te doy M me da la matriz que tiene,

397
00:41:15,060 --> 00:41:19,400
primera fila, uno, dos, tres, segunda fila, cuatro, cinco, seis, entonces la fila, si es tu chaval,

398
00:41:19,440 --> 00:41:28,980
así, acá lo que hice con esto de B fue definir la matriz B y como la definir

399
00:41:28,990 --> 00:41:36,020
igual, puse unos R y de 2 unos R y de 2 por I y así, ok?

400
00:41:40,480 --> 00:41:45,960
bueno, esto es lo que hice acá y fíjense

401
00:41:46,420 --> 00:41:50,080
acá estoy usando una función de "keySkit" que se llama "unitary"

402
00:41:54,480 --> 00:42:01,320
¿Qué hace? yo puedo poner una matriz "m", tengo que indicar sobre qué cubit actúa,

403
00:42:01,500 --> 00:42:05,680
el cubit 1, el cubit 2, el cubit 3, acá le estoy diciendo que actúe en el 0,

404
00:42:06,920 --> 00:42:13,100
yo lo estoy llamando B para la matriz y le pongo un label, una etiqueta

405
00:42:16,020 --> 00:42:21,740
me podrías poner por ahí Federico o etiqueto o J, este tipo de nombres de etiqueta

406
00:42:23,520 --> 00:42:29,620
que hago con esto, bueno, le estoy diciendo que al circuito MZ le aplique la unitaria

407
00:42:29,920 --> 00:42:33,780
definida arriba que es la "b" en el "Cubit 0"

408
00:42:34,640 --> 00:42:39,920
"b" es un "Pia Rai" la matriz y le digo a "Kiskit"

409
00:42:39,980 --> 00:42:46,020
que le aplica al "Cubit 0" la matriz "b" y que lo dibuje con este label

410
00:42:49,460 --> 00:42:54,920
bien y acá al mismo circuito le agregué esta fase

411
00:42:56,620 --> 00:43:02,460
yo esta fase la podría haber definido igual que acá, podría haber definido una matriz, vamos a hacerlo

412
00:43:07,940 --> 00:43:09,660
vamos a hacer una matriz de 2 por 2

413
00:43:17,480 --> 00:43:19,560
p igual a np array

414
00:43:21,180 --> 00:43:24,920
entendemos que ponemos uno acá, un 0 acá

415
00:43:28,260 --> 00:43:31,920
acá un 0 y acá un...

416
00:43:34,800 --> 00:43:36,940
¿Cómo sería? Che, npx...

417
00:43:40,900 --> 00:43:44,400
j1 por j por una fase phi

418
00:43:47,160 --> 00:43:50,780
algo así, o no, che, por qué no me...

419
00:43:53,260 --> 00:43:56,660
bien donde phi es una fase que vamos a tener que definir

420
00:43:57,680 --> 00:44:03,200
bueno, le puse fase, phi es igual a 0,5, lo que sea, un numerito

421
00:44:06,900 --> 00:44:09,440
y acá me pasó que me olvide cerrar un par de veces

422
00:44:10,000 --> 00:44:15,920
me caí, bccode, me indica que me equivoqué

423
00:44:15,920 --> 00:44:18,600
Bueno, se entiende esto? Alguna pregunta?

424
00:44:20,440 --> 00:44:21,400
O sea, lo...

425
00:44:21,850 --> 00:44:26,020
¿Está poniendo la matriz como una consiste en otro ejemplo?

426
00:44:27,119 --> 00:44:28,560
Claro, como en "V"

427
00:44:30,260 --> 00:44:33,320
Lo escribí, se lo estoy mostrando solo para que vean cómo se hace.

428
00:44:34,619 --> 00:44:36,060
Pero, pero...

429
00:44:36,340 --> 00:44:36,760
La borro.

430
00:44:37,660 --> 00:44:45,900
¿Por qué? Porque...

431
00:44:45,900 --> 00:44:54,660
que se llama P, esto también es importante que lo incorpore ¿no?

432
00:44:55,900 --> 00:44:56,700
"Pgate"

433
00:44:59,240 --> 00:45:00,040
"Facegate"

434
00:45:03,600 --> 00:45:09,320
"Varei" y acá les dice cómo son los métodos para aplicar la compuesta P

435
00:45:09,900 --> 00:45:19,400
la función es p y representa, tiene un input que es el ángulo y eventualmente el qubits sobre el

436
00:45:19,440 --> 00:45:31,440
cual actúa y representa matemáticamente a esta matriz, ok? entonces saca esta misma p,

437
00:45:31,440 --> 00:45:40,840
si se fijan esto es lo que yo tengo en mi idea positivo es esto acá, es a la idelta,

438
00:45:41,000 --> 00:45:49,000
bueno ahí le llaman tita, ella es la idelta, yo le llame ps bueno en kiskis se llama p pero

439
00:45:49,060 --> 00:45:55,180
esta comporta ya está built in, ya está construida adentro de kiskis, no la tiene que armar ustedes,

440
00:45:55,280 --> 00:46:04,120
esta otra no estaba como estaba por esta aquello pero el puerto esta otra

441
00:46:04,380 --> 00:46:11,580
armello a mano, ¿entienden? arméon militar y cómo le aplicó a la carne y con esta función unitar

442
00:46:14,700 --> 00:46:17,320
bien entonces esta línea es

443
00:46:21,640 --> 00:46:25,040
El efecto del primer divisor de os.

444
00:46:27,940 --> 00:46:30,240
- Perfecto. - As, as, no, as.

445
00:46:32,410 --> 00:46:35,580
- Sí, está bien. - ¿Está bien? ¿Están seguras?

446
00:46:36,540 --> 00:46:41,280
- Sí, porque en plural lo aconchén entonces en singular lo aconchén.

447
00:46:42,160 --> 00:46:45,840
- OK, bueno. Me muero de vergüenza, no importa.

448
00:46:46,360 --> 00:46:53,100
acá este M, esta es la fase intermedia, el face shifter, es que estamos llamando face shifter

449
00:46:53,440 --> 00:46:53,580
¿sí?

450
00:46:55,400 --> 00:47:00,280
y este sería el de vuelta al segundo divisor de As

451
00:47:02,720 --> 00:47:05,480
No, me equivoco yo, me parece que es con...

452
00:47:05,560 --> 00:47:05,820
¿viste?

453
00:47:06,380 --> 00:47:08,260
Porque As es de hacer, es de hacer

454
00:47:08,620 --> 00:47:09,880
Por eso es hacer, por eso

455
00:47:10,300 --> 00:47:11,340
No, pero tampoco es así

456
00:47:11,700 --> 00:47:13,360
No, es con Z, As de luz es con Z

457
00:47:14,360 --> 00:47:15,860
pero sin H. ¿Has

458
00:47:44,360 --> 00:47:51,440
y detectores y acá les digo que le grafique grafica lo corremos

459
00:47:59,380 --> 00:48:01,520
que uro gracias por que tardó tanto

460
00:48:03,880 --> 00:48:11,560
bueno y esto es lo que yo había dibujado en el en el acá en la

461
00:48:14,180 --> 00:48:19,020
esto es esto, lo reconocen? BC1, PSDS2

462
00:48:24,200 --> 00:48:29,020
¿Por qué les cuento esto? Para que vean cómo es la lógica de construcción de un circuito

463
00:48:29,680 --> 00:48:30,480
Eso es lo que estamos haciendo

464
00:48:32,800 --> 00:48:39,080
Este sería BC1, P, acá P, definió una variable fase

465
00:48:39,080 --> 00:48:43,920
que le puede dar el valor que quiera, que yo p/5, o sea, lo que quiera

466
00:48:48,300 --> 00:48:50,020
y con eso me damos el circuito

467
00:48:54,100 --> 00:49:00,940
y ven que, acá si le ponía, en vez del A, del B, le ponía un F, a ver si no tomó

468
00:49:08,260 --> 00:49:09,060
F, ven

469
00:49:12,280 --> 00:49:17,000
esto se lo digo para que vean que ustedes pueden con esto introducir

470
00:49:20,260 --> 00:49:23,120
introducir la comporta lógica que quieran

471
00:49:29,820 --> 00:49:34,060
y con esta función le ponen una etiqueta

472
00:49:36,060 --> 00:49:40,480
y dicen en qué qubit actúa.

473
00:49:41,680 --> 00:49:44,040
Acá como hay un qubit, siempre se esquilce.

474
00:49:45,180 --> 00:49:45,980
Alguna pregunta?

475
00:49:49,360 --> 00:49:52,420
El ángulo de la fase en que influye.

476
00:49:53,960 --> 00:49:54,880
Ahora lo vamos a ver.

477
00:49:56,600 --> 00:49:58,660
Es lo interesante de todo esto.

478
00:49:59,540 --> 00:50:01,060
Pero ya llegaremos en breve.

479
00:50:02,760 --> 00:50:03,680
Ahora te lo digo.

480
00:50:04,400 --> 00:50:11,020
para y otra cosa pero bueno ven que tenemos tres cosas una cosa es el

481
00:50:11,380 --> 00:50:14,680
circuito pero el experimento que es esto de acá

482
00:50:18,220 --> 00:50:24,520
y acá tenemos esta explicación secuencial que corresponde a que cada vez

483
00:50:24,540 --> 00:50:31,520
que mete una compuerta significa multiplicar al estado por una matriz que

484
00:50:31,520 --> 00:50:38,880
esto de acá, multiplico, multiplico, se entiende? Y acá tenemos el circuito, donde el tiempo va en la

485
00:50:39,000 --> 00:50:45,480
dirección de esta flecha. Esa es la lógica de construcción de circuitos. Todas las plataformas

486
00:50:45,750 --> 00:50:53,200
de desarrollo de código para computar las cuánticas son más o menos así. Uno, tiene estado cuántico

487
00:50:53,480 --> 00:51:01,080
y le va aplicando con portas unitarias que lo van transformando. ¿Y qué tiene que hacer? Y bueno,

488
00:51:02,119 --> 00:51:04,440
indicarle a estas comportas de que Qubes

489
00:51:04,700 --> 00:51:07,360
actúan y en que ahora no.

490
00:51:10,400 --> 00:51:16,940
Ok? Fíjense que el otro circuito el que no tenía

491
00:51:19,760 --> 00:51:22,700
va a ser otro que no tiene su logo implíter

492
00:51:49,300 --> 00:51:51,119
Esto de igual nada más que...

493
00:51:54,200 --> 00:51:56,360
no le ponemos el segundo de visor de as

494
00:52:02,520 --> 00:52:05,340
este sería sin poner el segundo de visor de as,

495
00:52:07,380 --> 00:52:13,560
entonces a este experimento no vamos a referir experimento tipo onda y a este experimento tipo

496
00:52:13,640 --> 00:52:19,840
particular ahora va a quedar claro por qué hay dos circuitos una asociada a cada contexto de

497
00:52:19,840 --> 00:52:27,760
de edición. Bueno, alguna pregunta, yo les cuento todo esto para que vean cómo es la lógica

498
00:52:27,760 --> 00:52:32,900
de construcción de circuitos, porque si hace un circuito más complejo va a ser igual,

499
00:52:33,100 --> 00:52:38,640
es la misma idea. Tienen los qubits y sobre los qubits van aplicando corporta. La cosa

500
00:52:38,720 --> 00:52:44,840
se lee de izquierda a derecha y cada vez que aplican una matriz significa que el estado

501
00:52:44,840 --> 00:52:48,420
de edición lo va multiplicando primero por esta matriz, de izquierda a derecha, después

502
00:52:48,420 --> 00:52:56,440
por esto, después por esto. Sí. Yo tengo una pregunta respecto al Beam Splitter,

503
00:52:56,760 --> 00:53:02,360
cómo está modelado. Introduce una fase en el reflejado, no? Una fase de 90,

504
00:53:02,640 --> 00:53:09,460
el Beam Splitter en el reflejado. Y ahí, vos, en el primer Beam Splitter que pones, bueno,

505
00:53:09,780 --> 00:53:14,560
se la introducís, digamos, al que va para arriba, a la fase 90, porque ese es el que se refleja,

506
00:53:14,560 --> 00:53:22,600
y en el segundo beam splitter se está aplicando al correcto o no la fase 90. Lo que pasa es que,

507
00:53:23,480 --> 00:53:33,720
la entiendo, no porque esa compuerta ya tiene eso incorporado, que el que se refleja tiene una

508
00:53:33,720 --> 00:53:40,960
de 90, cuando las cosas entran en segundo beam splitter, bueno, sabes, se va a reflejar o transmitir.

509
00:53:42,020 --> 00:53:44,260
Entonces, ¿tendrías que aplicar la misma operación de vuelta?

510
00:53:45,560 --> 00:53:50,580
Claro, mi duda es, porque esto es como que rompe la simetría entre el primero y el segundo,

511
00:53:50,720 --> 00:53:52,540
entre el que se refleja y el que no se refleja.

512
00:53:52,720 --> 00:53:59,280
Entonces, ¿no estaba seguro si ya está respetado eso al armar el circuito de esa manera?

513
00:54:00,900 --> 00:54:05,540
Yo creo que está respetado. No veo bien por qué decir que se rompe,

514
00:54:05,960 --> 00:54:12,260
el que se refleja, no pasa que a nivel cuántico ni se reflejan ni no se reflejan.

515
00:54:16,140 --> 00:54:21,620
Claro, ¿cuál de los dos le aplicas la fase de 90, digamos al estado 0 o al estado 1? En el

516
00:54:21,640 --> 00:54:24,880
primero veo claramente que se le aplicas al estado 1 digamos.

517
00:54:28,080 --> 00:54:41,440
lo que pasa es que este segundo va a optar sobre una combinación ideal

518
00:54:44,800 --> 00:54:47,780
porque vas a tener que hacer a ver si me dejes que diga a caro

519
00:54:50,320 --> 00:54:50,940
se queda haciendo

520
00:54:50,980 --> 00:55:00,840
no, no hay que hablar de

521
00:55:22,059 --> 00:55:33,020
es este por 0 y si entran así lo llamas 1 es este por 1, pero no importa como lo llames

522
00:55:33,810 --> 00:55:38,760
lo que importa es que tenés un espacio vectorial y a la salida del primer divisor de as

523
00:55:40,380 --> 00:55:42,980
voy a hacer una superpunción que es esta de acá

524
00:55:52,200 --> 00:55:54,740
esta, que esta es la fase que vos decís que le aplicó

525
00:55:55,980 --> 00:55:57,600
y ahora lo haces de vuelta

526
00:56:00,420 --> 00:56:03,560
es como que a la salida del primer divisor de as

527
00:56:04,040 --> 00:56:08,300
el fotón quedó en una superpunción entre modo 0 y modo 1

528
00:56:09,319 --> 00:56:15,260
no está ninguno de los dos, está en la superposición, cuando vos lo vuelvas

529
00:56:15,360 --> 00:56:20,780
aplicar al disordaz, opera linealmente, ¿me se veis?

530
00:56:22,140 --> 00:56:22,220
si

531
00:56:25,280 --> 00:56:31,060
bueno después también ocurre esta fase del medio y vos volves a aplicar ahí

532
00:56:31,250 --> 00:56:36,300
y operar sobre cada término de la superposición

533
00:56:37,160 --> 00:56:39,520
básicamente el bs2 acá a la postcript

534
00:56:40,900 --> 00:56:43,940
lo voy a pensar un poquito más pero nada bien

535
00:56:47,860 --> 00:56:51,640
lo voy a pensar yo también a ver qué es esto que me estás diciendo

536
00:56:51,900 --> 00:56:53,420
a ver si se rompe o no lo hace de teguín

537
00:56:54,220 --> 00:56:57,660
pero si es verdad que ese "i" tiene que ver con que el que se refleja

538
00:56:57,660 --> 00:57:01,300
se lleve una fase y medio que lo estás contemplando acá

539
00:57:04,300 --> 00:57:13,100
bien, entonces volviendo a la representación del circuito

540
00:57:16,660 --> 00:57:21,140
empezábamos con el estado cero y a la salida teníamos un estado que creo que le

541
00:57:21,300 --> 00:57:24,520
llamé si 3 ok y sobre este estado medimos

542
00:57:26,740 --> 00:57:27,720
se llama si 3

543
00:57:34,840 --> 00:57:35,940
Sí, sí te les le llaman.

544
00:57:38,540 --> 00:57:42,040
Este es el estado final, les queda como ejercicio probar esto.

545
00:57:42,770 --> 00:57:51,500
En realidad acá hay una cuenta que acá aplique el típico truco de sacar factor común.

546
00:57:53,400 --> 00:57:58,960
Déjenme hacerlo acá, afuera, en la pizarra porque alguna le va a salir.

547
00:58:02,000 --> 00:58:07,180
si 3 se se iguala un medio por una menospera y el tamas y pute

548
00:58:29,320 --> 00:58:30,200
por 1

549
00:58:32,940 --> 00:58:34,160
no se me ha de la

550
00:58:59,080 --> 00:59:03,540
menos y delta sobre 2 menos e a la i delta sobre 2.

551
00:59:05,690 --> 00:59:07,920
Es el típico truco de sacar factor común

552
00:59:08,150 --> 00:59:12,040
a lo que no está tan evidentemente con factor común.

553
00:59:13,620 --> 00:59:16,860
Pero si se fijan esto de abajo es esto de arriba,

554
00:59:17,160 --> 00:59:22,580
porque si vuelvo a multiplicar este por este me da e a la i delta sobre 2,

555
00:59:22,840 --> 00:59:24,600
por e a la menos y delta sobre 2 es 1.

556
00:59:25,720 --> 00:59:30,720
y E a la...

557
00:59:33,040 --> 00:59:35,640
Claro, y delta sobre 2 por E a la y delta sobre 2,

558
00:59:35,660 --> 00:59:36,820
es E a la y delta, ¿sí?

559
00:59:37,720 --> 00:59:39,280
Entonces ahí saque factor común este

560
00:59:39,440 --> 00:59:41,060
y en este hago algo muy parecido.

561
00:59:42,380 --> 00:59:42,860
Hago...

562
00:59:42,860 --> 00:59:45,020
A esto de acá, lo reescribo como

563
00:59:46,520 --> 00:59:49,220
E a la y delta por...

564
00:59:49,220 --> 00:59:51,920
Delta, perdón, sobre 2 por...

565
00:59:51,920 --> 00:59:57,020
a la menos y del tazorreos más y a la y del tazorreos.

566
00:59:57,620 --> 00:59:57,700
Ok?

567
00:59:58,740 --> 01:00:03,140
Y ahora tengo el e ala y del tazorreos en los dos términos y nos saco factor común.

568
01:00:04,900 --> 01:00:14,000
Bueno, importante, hagan esto en su casa porque es algo de fácil, pero si no lo hacen y no

569
01:00:14,000 --> 01:00:18,260
lo piensan rato es completamente misterioso y no se te da nada.

570
01:00:19,260 --> 01:00:26,420
pero bueno, de acá a acá hice eso, saqué factor con un e a la y del tazoreros

571
01:00:30,039 --> 01:00:32,380
bien primera cosa primera cosa

572
01:00:36,020 --> 01:00:39,880
este e a la y del tazoreros es una fase global

573
01:00:42,680 --> 01:00:45,520
vamos a volver acá

574
01:00:47,680 --> 01:00:52,060
la grasa es ésta, supongan que tienen un estado cuántico que es

575
01:00:54,559 --> 01:00:56,020
si igual a

576
01:00:58,080 --> 01:01:03,200
si prima, ya os leé, si prima igual a e a la i delta por si

577
01:01:06,200 --> 01:01:06,400
¿sé?

578
01:01:09,840 --> 01:01:13,180
¿Qué pasa si ha dado si prima contra si?

579
01:01:16,680 --> 01:01:18,920
para cualquier phi, módulo al cuadrado.

580
01:01:20,960 --> 01:01:24,700
Esto era la probabilidad de transición de "psi" prima a "phi".

581
01:01:27,420 --> 01:01:33,660
Esto les dejo como ejercicio comprobar que es módulo de "e" a la "i" delta

582
01:01:37,760 --> 01:01:42,800
por módulo de "psi" contra "phi" al cuadrado.

583
01:01:44,040 --> 01:01:47,780
y como el módulo de "y" a la "y" delta es igual a 1,

584
01:01:50,360 --> 01:01:58,740
esto me queda módulo de "c" con "f" al cuadrado y esto me queda probabilidad de "psi" a "fi".

585
01:01:59,400 --> 01:02:03,920
¿Qué quiere decir esto? Que si un estado nuevo

586
01:02:04,500 --> 01:02:11,300
se obtiene a partir de un viejo estado, a partir de multiplicarlo por una fase compleja,

587
01:02:11,480 --> 01:02:20,700
por un E, un exponencial de I, Delta, la probabilidad de transición del nuevo estado a cualquier

588
01:02:20,700 --> 01:02:24,500
otro estado es igual a la probabilidad de transición del viejo estado.

589
01:02:26,040 --> 01:02:33,020
Entonces, esto implica que la física del problema no cambia por multiplicar a un estado por

590
01:02:33,080 --> 01:02:33,980
una fase global.

591
01:02:34,040 --> 01:02:40,040
es decir, si yo hago un "psi" y lo multiplico por "m" y "delta", el estado cuántico es

592
01:02:40,140 --> 01:02:47,240
exactamente el mismo, físicamente. El vector es diferente porque matemáticamente lo multiplico

593
01:02:47,260 --> 01:02:55,080
por otro estado. Pero el estado cuántico, no. Ok? Entonces, el estado cuántico queda definido

594
01:02:55,130 --> 01:03:01,160
a menos de una fase global. Es algo que tiene que recordar porque va a parecer más adelante.

595
01:03:06,480 --> 01:03:10,660
Y es importante distinguir la fase global de una fase local porque si yo por ejemplo

596
01:03:11,080 --> 01:03:22,960
0 más e a la y phi por 1 sobre el raíz de 2 y esto lo llamo delta vamos a ponerle perdón a fase

597
01:03:30,420 --> 01:03:37,760
y esto lo llamo psizubdelta cuando cambie delta a casi va a cambiar el estado físicamente va a

598
01:03:37,760 --> 01:03:44,700
cambiar pero si la fase la pongo acá adelante y a la dienta no cambia nada ok?

599
01:03:45,980 --> 01:03:46,840
ese es el mensaje

600
01:03:50,700 --> 01:03:52,880
la fase global no cambia el estado del sistema

601
01:03:56,960 --> 01:04:02,920
bien, o sea acá me quedó una fase de verdad y por qué hice todo este tejer y

602
01:04:02,920 --> 01:04:09,880
maneje de reescribir todo así, bueno, porque ahora podemos usar las identidades

603
01:04:10,060 --> 01:04:20,540
trionamétricas, lo escribo acá. Se sabe que se puede probar que e a la i

604
01:04:21,180 --> 01:04:29,760
delta sobre 2 es coseno de delta sobre 2 más i por el seno de delta sobre 2.

605
01:04:30,920 --> 01:04:37,920
En general, e a la y fi es igual a cosena de fi más y por el seno de fi.

606
01:04:39,760 --> 01:04:40,960
Esta es la regla que usamos.

607
01:04:42,500 --> 01:04:51,900
Entonces, fíjense que si usan eso, si usan esta regla de acá,

608
01:04:53,440 --> 01:04:57,120
pueden reescribir esto de acá entre el mío de un seno y un coseno.

609
01:05:02,940 --> 01:05:07,740
¿Por qué? ¿Por qué? Sí, alguien ahí quiere preguntar algo, decir algo. Adéu ante.

610
01:05:10,160 --> 01:05:15,960
Pérez, a mí en algún momento se me ocurrió, pero no sé si de pronto ya se había trabajado con eso.

611
01:05:16,020 --> 01:05:23,660
Si se puede escribir en términos de ser el coseno, existiría como algún desarrollo matemático relacionado con furiero?

612
01:05:24,240 --> 01:05:26,900
o eso acá no tiene como una aplicación directa.

613
01:05:28,160 --> 01:05:28,800
Si me vas a entender.

614
01:05:30,840 --> 01:05:35,800
No, a ver, esa formulita la puedes calcular, puedes tomar como una definición, tipo

615
01:05:36,140 --> 01:05:41,460
"Ela, I, F, es igual a esto" o podrías hacer la serie de potencias, la serie de Taylor,

616
01:05:42,400 --> 01:05:48,460
del coseno y vas a llegar, no, perdón, de la exponencial y vas a llegar a eso, entiendes?

617
01:05:49,420 --> 01:05:50,240
Es una gran...

618
01:05:51,080 --> 01:05:55,840
sobre lo que es hacer lo mismo si me hubieras que hacer eso, con el celdo, la matriz, etc.

619
01:05:57,340 --> 01:06:02,440
Después acá justo no aplica furiel porque estamos en la dimensión finita, pero en la

620
01:06:02,480 --> 01:06:10,900
dimensión finita si todo el tiempo, típicamente vas a hacer, puedes reescribir a tu estado,

621
01:06:11,480 --> 01:06:11,660
¿viste?

622
01:06:12,780 --> 01:06:18,640
Ok, elegante, dale, es que yo día estar aquí, de pronto ya lo han hecho, entonces muy bien,

623
01:06:19,240 --> 01:06:26,680
gracias. No, si, si, si, y además fíjate la realidad va a ser esto, suponerte que vos tenés L2,

624
01:06:27,260 --> 01:06:38,160
viste, el conjunto de los F que van de reales a los complejos tales que el modo WF, no,

625
01:06:38,160 --> 01:06:50,380
que el integral del módulo de f al cuadrado es menor que infinitos, L2, bien, si usted

626
01:06:51,500 --> 01:07:04,480
si haces f por g como un producto interno se definís así, f por g conjugado de x, esto

627
01:07:04,480 --> 01:07:12,900
final un producto interno y vos te venís con alguna base de D2 la que sea vos pues a cualquier

628
01:07:13,240 --> 01:07:21,640
F la vas a poder escribir como como proyectando coordenadas entendés y al final furiar lo

629
01:07:21,760 --> 01:07:28,920
podés pensarme de así no se dice en el vídeo. Sí, sí claro claro, ya se tomó una base de D2

630
01:07:29,720 --> 01:07:37,380
digamos que la escena o cosena y con esa base orto normal se puede creer cualquier función de

631
01:07:37,380 --> 01:07:44,580
ahí de como una serie. Justo el escena o cosena no son una base porque un seno no

632
01:07:44,640 --> 01:07:49,100
pertenece a la edad, no puede ser. Pero la idea es esa.

633
01:07:51,540 --> 01:07:53,120
Sí, pues dale, gracias. Muy bien.

634
01:07:53,730 --> 01:08:01,480
Es decir, si al final vos lo que vas a hacer, vas a estar haciendo es proyectando alguna

635
01:08:01,640 --> 01:08:04,540
suerte de base o cosa que genere, viste que anda todo.

636
01:08:05,539 --> 01:08:08,940
Reciéndome yo, me informa, como lo digo, pero le dices esa.

637
01:08:09,350 --> 01:08:12,060
Y ese es la gracia de los espacios de Hitler, de algún modo que vos,

638
01:08:12,300 --> 01:08:21,540
vas a poder heredar todas las propiedades geométricas que tenías en R3 y CN a un espacio funcional, por ejemplo.

639
01:08:25,259 --> 01:08:27,279
Bien, volviendo a esto.

640
01:08:28,600 --> 01:08:36,700
Fede, una pregunta, ¿dónde la clase pasada y el código que estás trabajando, en qué parte exactamente el campo está el código de Python?

641
01:08:40,299 --> 01:08:40,620
パラン

642
01:08:47,100 --> 01:08:50,400
3種類

643
01:09:10,799 --> 01:09:11,060
acá

644
01:09:13,540 --> 01:09:17,380
hay una carpetita de principio todo que dice que después subo los de hoy

645
01:09:20,880 --> 01:09:22,380
ok ok listo listo bien

646
01:09:27,019 --> 01:09:33,980
bueno entonces haciendo esta cuenta me queda que la probabilidad la probabilidad

647
01:09:35,279 --> 01:09:40,980
de observar a cero, tengo que hacer el bracket de cero contra psitres,

648
01:09:42,220 --> 01:09:48,180
vamos con el estado final y esto les queda de ejercicio, cuando dan esta

649
01:09:48,240 --> 01:09:53,180
cuenta les queda que la probabilidad es el módulo del cuadrado, no perdón, el

650
01:09:53,380 --> 01:09:57,800
cero al cuadrado de la fase que introdujo el phase shifter sobre los

651
01:09:58,600 --> 01:10:01,560
y la probabilidad de detectar el mundo es el cocin del cuadrado

652
01:10:04,420 --> 01:10:10,700
entonces acá les pido que lo vuelvan a hacer esto y reflexionen sobre cómo se calcula la probabilidad

653
01:10:10,880 --> 01:10:12,600
acá estoy usando la rilesa

654
01:10:14,600 --> 01:10:15,580
yo cuando hago

655
01:10:23,500 --> 01:10:28,440
módulo de 0 contra c3 al cuadrado

656
01:10:28,880 --> 01:10:34,040
esto es la probabilidad de dado que el sistema está en c3

657
01:10:34,330 --> 01:10:36,280
yo lo detecte en cero, ¿sí entiendes?

658
01:10:37,600 --> 01:10:38,380
se calcula así

659
01:10:41,760 --> 01:10:47,720
ahí usé esta regla con una acción, una acción más de la, de la cuarta, la regla 2

660
01:10:53,100 --> 01:10:58,900
entonces así calculé esto y como lo hice bueno, haciendo todas las composiciones

661
01:10:59,440 --> 01:11:00,060
cero y cincocin

662
01:11:02,520 --> 01:11:07,760
bien y la gracia de esto es que cuando vayan variando y que quiere decir esto, piensen una cosa

663
01:11:07,760 --> 01:11:10,500
Piensen ahora en física de todo esto.

664
01:11:11,640 --> 01:11:13,880
O al menos cómo se podría interpretar.

665
01:11:15,860 --> 01:11:20,640
Tengo el primer binpliter, primer espejo, segundo espejo,

666
01:11:21,140 --> 01:11:22,300
segundo binpliter, ¿no?

667
01:11:22,540 --> 01:11:24,460
Detector de uno y detector de dos.

668
01:11:28,940 --> 01:11:34,740
Entonces, yo tirando fotones y van a ir impactando en de uno y

669
01:11:34,740 --> 01:11:35,260
de dos, ¿no?

670
01:11:35,400 --> 01:11:45,780
decíamos. Tengo una cuenta, otra cuenta, otra cuenta, otra cuenta. Entonces yo le voy a tener

671
01:11:46,180 --> 01:11:50,800
es que los fotones por unidad de tiempo van a ir cayendo, entonces nada que haga el que yo.

672
01:11:51,600 --> 01:11:56,100
En de uno, tanto fotones por segundo y en de dos, tanto fotones por segundo,

673
01:11:56,340 --> 01:12:00,960
pues yo le voy a ir repitiendo a los fotones muchas veces, millones de veces, las que sea.

674
01:12:03,420 --> 01:12:08,480
Entonces lo que voy a tener es una probabilidad de detección por unidad de tiempo.

675
01:12:09,230 --> 01:12:12,620
Voy a fijar cuántos fotones caen por segundo en ningún video.

676
01:12:12,960 --> 01:12:17,440
Entonces esa probabilidad va a ser proporcional a P1 y P2.

677
01:12:18,680 --> 01:12:18,900
Ok?

678
01:12:19,680 --> 01:12:30,900
La probabilidad esta cuántica P1 y P2 o el número de fotones que yo detecte por unidad de tiempo

679
01:12:30,900 --> 01:12:33,360
va a ser proporcional a P1 y a P2.

680
01:12:33,700 --> 01:12:40,220
Entonces, lo que van a observar en el laboratorio es que la intensidad de detección

681
01:12:40,300 --> 01:12:46,140
prioridad de tiempo, las 10 fotones que detectan prioridad de tiempo, oscila como

682
01:12:46,140 --> 01:12:49,260
el seno y el coseno al cuadrado cuando van cambiando la fase.

683
01:12:50,190 --> 01:12:57,060
Entonces, si tienen una fase, van a haber fases en las cuales todos se detectan de 1 y nada

684
01:12:57,060 --> 01:13:06,460
se detectan de 0, o si, y van a ver fases donde se detecta a mitad y a mitad, y van a ver fases donde se detectan

685
01:13:06,460 --> 01:13:12,840
en revés. ¿Se entienden esto? Es decir, ustedes observando la tasa de detección de

686
01:13:12,860 --> 01:13:20,300
fotones por un día de tiempo, van a dar un patrón de interferencia, a medida que van ajustando la

687
01:13:20,300 --> 01:13:28,980
fase del experimento. Esa es la idea. Entonces, qué es eso? Si le ponen phi, la delta igual

688
01:13:29,060 --> 01:13:37,300
a pi sobre 2, van a tener mi tinita. Si le ponen y van a detectar así, esto dice conquistir.

689
01:13:40,360 --> 01:13:47,100
Si le ponen fase igual a pi, van a tener que todo cae en un detector y nada en el otro

690
01:13:47,100 --> 01:13:47,580
ya se sigue

691
01:13:51,440 --> 01:13:52,320
con este código

692
01:13:55,080 --> 01:13:56,200
esto se puede calcular acá

693
01:13:57,820 --> 01:13:59,360
ahora lo mando a correr

694
01:13:59,760 --> 01:14:03,140
lo mando a correr a una computadorita cuántica

695
01:14:04,000 --> 01:14:04,540
ficticia

696
01:14:06,400 --> 01:14:07,340
y hago las cuentas

697
01:14:16,780 --> 01:14:22,760
y pueden jugar, yo después le paso la planilla esta y pueden jugar ir cambiando la fase

698
01:14:24,070 --> 01:14:28,200
y ruiendo como cambie la probabilidad en función de la fase

699
01:14:33,900 --> 01:14:35,260
no estaba descambiando

700
01:14:41,440 --> 01:14:41,680
bien

701
01:14:49,660 --> 01:14:57,800
Bueno, y por último, para terminar esta primera parte, es importante comentar qué pasaría

702
01:14:58,160 --> 01:15:05,320
si no ponemos el segundo divisor de As, si no ponemos el segundo divisor de As, lo que

703
01:15:05,480 --> 01:15:10,380
obtenemos es que la probabilidad es un medio y un medio, independientemente de la fase,

704
01:15:10,960 --> 01:15:11,660
si se puede calcular

705
01:15:12,860 --> 01:15:13,860
lo tenemos acá

706
01:15:16,940 --> 01:15:19,460
¿Por qué? Bueno, porque tengo que hacer...

707
01:15:21,280 --> 01:15:22,720
ahora ya lo pongo el segundo

708
01:15:23,100 --> 01:15:25,360
y implica, entonces el estado de la salida es fidos

709
01:15:29,180 --> 01:15:31,580
entonces cuando hago la probabilidad acá

710
01:15:33,260 --> 01:15:36,960
voy a encontrar que no me depende de la fase

711
01:15:36,960 --> 01:15:45,540
eso también lo pueden hacer como ejercicio, tienen que si no pongo el segundo

712
01:15:45,660 --> 01:15:51,020
de un clíter entonces y a qué se corresponde eso bueno se corresponde una

713
01:15:51,060 --> 01:15:52,240
situación en la cual

714
01:16:00,380 --> 01:16:03,700
o será que esta sería la situación que había dicho antes que sería algo muy

715
01:16:03,700 --> 01:16:04,000
que se están

716
01:16:34,900 --> 01:16:41,200
la probabilidad iba como un 0 cuadrado y coseno cuadrado y ahí decías que hay interferencia

717
01:16:41,440 --> 01:16:48,240
en función de qué? de la diferencia de fase que introduce el phase shifter, si vos no pones el

718
01:16:48,460 --> 01:16:55,160
segundo divisor de as, solo vas a ver que la mitad de los fotones van a parar el detector y la

719
01:16:55,220 --> 01:16:59,700
otra mitad va a parar el detector y listo, no importa la fase que le pongas al phase shifter,

720
01:16:59,740 --> 01:17:01,580
no vas a ver interferencia, ¿entendés?

721
01:17:02,920 --> 01:17:03,100
Claro

722
01:17:10,900 --> 01:17:14,140
Bueno, esto era la primera parte

723
01:17:15,430 --> 01:17:19,380
y ahora en la segunda parte vamos a ver un ejemplo de un algoritmo cuántico

724
01:17:22,500 --> 01:17:25,740
Así que, nos vemos en 10 minutos

725
01:17:25,740 --> 01:17:26,300
si parece

726
01:17:26,740 --> 01:17:27,740
De un minuto de cuanto?

727
01:17:28,080 --> 01:17:28,540
D'accord.

728
01:17:29,800 --> 01:17:30,440
Voilà.

729
01:17:31,020 --> 01:17:31,960
Nous allons en faire un granditum.

730
01:17:32,860 --> 01:17:33,060
D'accord.

731
01:17:34,080 --> 01:17:44,080
[BLANK_AUDIO]

732
01:18:31,260 --> 01:18:34,060
Yn ymw

733
01:19:01,260 --> 01:19:04,060
Yn ymw

734
01:19:31,260 --> 01:19:34,060
Yn ymw

735
01:19:59,100 --> 01:20:01,900
Yn ymw

736
01:20:31,260 --> 01:20:34,060
Yn ymw

737
01:21:01,260 --> 01:21:04,060
Yn ymw

738
01:21:29,100 --> 01:21:31,900
Yn ymw

739
01:22:01,260 --> 01:22:04,060
Yn ymw

740
01:22:29,220 --> 01:22:32,020
Yn ymw

741
01:23:01,260 --> 01:23:04,060
Yn ymw

742
01:23:31,260 --> 01:23:34,060
Yn ymw

743
01:24:01,260 --> 01:24:04,060
Yn ymw

744
01:24:29,000 --> 01:24:31,800
Yn ymw

745
01:24:34,080 --> 01:25:04,060
Yn ymw

746
01:25:31,260 --> 01:25:34,060
Yn ymw

747
01:25:59,140 --> 01:26:01,940
Yn ymw

748
01:26:31,260 --> 01:26:34,060
Yn ymw

749
01:26:59,140 --> 01:27:01,940
Yn ymw

750
01:27:29,100 --> 01:27:31,900
Yn ymw

751
01:27:59,100 --> 01:28:01,900
Yn ymw

752
01:28:31,260 --> 01:28:34,060
Yn ymw

753
01:28:59,140 --> 01:29:01,940
Yn ymw

754
01:29:26,739 --> 01:29:30,000
Bueno, ahí me ven y me escuchan, si no?

755
01:29:32,420 --> 01:29:41,580
ahora si, cambié dispositivo porque acá tengo una mejor... ahora ya no voy a hacer

756
01:29:41,680 --> 01:29:48,720
más códigos y acá tengo un mejor... como se llama un mejor pizarroncito, si quieres

757
01:29:48,840 --> 01:29:49,820
los puedo compartir

758
01:29:53,420 --> 01:29:57,020
esperen que estoy ahí

759
01:30:03,840 --> 01:30:05,020
ya comparto eh

760
01:30:05,840 --> 01:30:06,960
¿Te voy a guardar la pantalla?

761
01:30:21,960 --> 01:30:22,520
Bueno

762
01:30:25,920 --> 01:30:27,120
¿Te ve la pantalla ahí, no?

763
01:30:28,940 --> 01:30:29,580
Sí, profe.

764
01:30:31,840 --> 01:30:37,320
Bien, entonces, nada bueno, ahora vamos a hacer un pequeño repaso matemático

765
01:30:39,120 --> 01:30:44,220
y vamos a ver después un primer ejemplo del barismo cuántico

766
01:30:49,660 --> 01:30:52,920
Bueno, no entiendo por qué estas tratan de encargar

767
01:30:56,680 --> 01:30:59,840
Bueno, por las dudas hablo uno de estos pizarrones

768
01:31:01,280 --> 01:31:29,460
ი ი ი ი ი ი ი ი ი ი ი ი ʁი იიი ი ი �

769
01:31:52,760 --> 01:31:54,160
*cantando*

770
01:31:55,360 --> 01:31:56,400
que huracate

771
01:32:26,700 --> 01:32:26,840
Ahí.

772
01:32:45,840 --> 01:32:55,460
Bien, bueno, recuerden que si queremos un qubits solo tiene el concepto de base, la base tiene

773
01:32:56,300 --> 01:33:02,980
12 elementos, en este caso 0 y 1, sería la base computacional y si tienen 2 qubits tienen que hacer el producto

774
01:33:03,080 --> 01:33:12,840
tensorian entre los estados de los qubits y eso les va a dar, para el caso de los 2 qubits, una base que tiene 4 elementos

775
01:33:13,420 --> 01:33:18,640
y así siguenlo, si tienen 3 qubits va a tener hecho elementos y así son todas las combinaciones posibles

776
01:33:21,260 --> 01:33:22,880
eso lo habíamos visto en la vez pasada

777
01:33:24,460 --> 01:33:32,480
y la otra cosa importante es el producto escalar, el producto escalar es eso que habíamos visto

778
01:33:35,940 --> 01:33:37,840
vamos a escribir en la pantalla un poquito

779
01:33:40,560 --> 01:33:43,600
se acuerdan que cuando teníamos la la psi contra phi,

780
01:33:44,440 --> 01:33:47,020
esto módulo del cuadrado era la amplitud de probabilidad, bueno,

781
01:33:47,840 --> 01:33:51,800
esto de acá es el reducto escalar, entonces uno pueda saber que es yo

782
01:33:52,020 --> 01:33:56,120
0 a 0 contra 0 a 1 y este va a dar 0, ¿por qué?

783
01:33:56,200 --> 01:33:59,720
porque esta bitstring no es la misma que esta, entonces

784
01:34:00,240 --> 01:34:03,460
si tiene una bitstring se hace así, esto da 1,

785
01:34:03,820 --> 01:34:08,340
cuando coinciden las bitstrings da 1, por ejemplo así,

786
01:34:08,340 --> 01:34:15,100
la 1 y cuando son distintas de alguna manera da 0 por ejemplo en este caso de acá

787
01:34:16,000 --> 01:34:23,220
tenemos 1 0 y 1 0, ahí da 1 el producto escalar, mientras que acá tenemos 1 0 y 0 1, las bits

788
01:34:23,400 --> 01:34:29,660
trings son distintas porque ahí cambia el orden, entonces este da 0 y así siguiendo y con 3 qubits

789
01:34:29,690 --> 01:34:38,320
es lo mismo por ejemplo acá tengo 1 0 0 contra 0 1 0 eso da 0 y 1 0 1 contra 1 solo 1 es decir

790
01:34:38,320 --> 01:34:39,340
el mismo vector de 1.

791
01:34:41,020 --> 01:34:44,280
Entonces cuando es la misma cadena, el producto escalar da 0.

792
01:34:46,900 --> 01:34:50,840
No, perdón. Cuando es la misma cadena, el producto escalar da 1.

793
01:34:51,160 --> 01:34:52,280
Y si no, da 0.

794
01:34:53,120 --> 01:34:54,300
¿Y por qué eso es importante?

795
01:34:54,600 --> 01:34:55,740
Bueno, por la regla de Born.

796
01:34:58,600 --> 01:35:03,320
Porque haciendo el producto escalar, calculan la amplitud de probabilidad

797
01:35:03,320 --> 01:35:07,480
y a partir de la amplitud de probabilidad calcula la probabilidad como el modo de la cuadrada.

798
01:35:09,000 --> 01:35:19,800
Bien, y en muchos sabidurismos cuánticos lo que van a encontrar es que le aplican la

799
01:35:19,860 --> 01:35:25,760
comporta hajamar a todos los qubits. Acá tenemos n qubits, acá este tensor a la n, lo voy a aclarar un poquito.

800
01:35:32,440 --> 01:35:41,660
digamos acá 0 a la n significa 0 tensor 0 tensor 0 n veces

801
01:35:45,280 --> 01:35:50,420
y esto nosotros lo poníamos en notación compacta como 0 0 0 n veces

802
01:35:52,540 --> 01:35:58,760
entonces este h a la n este tensor acá lo que significa es que aplican hadamar a cada uno de

803
01:35:58,760 --> 01:36:07,300
los qubits esto quiere decir por ejemplo si tuvieran 13s H tensor H, tensor H todo por

804
01:36:07,900 --> 01:36:22,520
0, tensor 0, tensor 0 y esto sería H por 0, tensor H por 0, tensor H por 0

805
01:36:25,080 --> 01:36:29,880
¿Sí? Y esto en términos de circuitos sería

806
01:36:30,700 --> 01:36:36,860
Hadamard al primer qubit, Hadamard al segundo qubit y Hadamard al tercer qubit, ¿OK?

807
01:36:39,020 --> 01:36:46,840
Entonces esta operación la van a ver muchas veces. H al AN, tensor 0 al AN, que es H por 0, tensor H por 0, tensor 8, ¿OK?

808
01:36:47,080 --> 01:36:53,980
y sería esto de acá, aplicarle "Hagamard" a cada uno de los quiblistos.

809
01:36:54,080 --> 01:37:00,480
Bien, si hacen eso les dejo como ejercicio comprobar que si hacen eso,

810
01:37:01,000 --> 01:37:05,100
si empiezan con el estado 0, digamos, esta de acá sería...

811
01:37:08,520 --> 01:37:25,780
esta acá sería h tensor 2 por 0 0 que sería h por 0 tensor h por 0 y bueno esto da esto da acá

812
01:37:25,940 --> 01:37:35,160
arriba, solo pueden hacer como ejercicio sencillo simplemente tienen que aplicar las definiciones

813
01:37:35,160 --> 01:37:39,500
de producto tensorial y lo que hace esta operatoria

814
01:37:46,120 --> 01:37:55,320
es producir este estado que lo que es es una combinación lineal de todos los

815
01:37:55,540 --> 01:38:00,440
elementos posibles de la base computacional y todo multiplicado por

816
01:38:00,480 --> 01:38:16,760
unos a la raíz de 4. Y si tuvieran 3 quebis, acá sería hhh, esperen.

817
01:38:26,220 --> 01:38:29,000
A nivel circuito sería esto, esto de acá arriba.

818
01:38:30,380 --> 01:38:36,520
También les da una superposición de todos los elementos de la base computacional de 3QB.

819
01:38:38,920 --> 01:38:40,560
Bueno, ¿y por qué esto es importante?

820
01:38:42,620 --> 01:38:49,160
Porque es un estado equiprobable, es decir, es un gato de Schrodinger, donde en vez de

821
01:38:49,160 --> 01:38:55,960
tener vivo y muerto tienen 0 0 0 o 1 0 0 o 0 1 0 y así las 8 posibilidades.

822
01:38:57,070 --> 01:39:00,520
¿Y cómo hacer por ejemplo para calcular la probabilidad acá?

823
01:39:04,420 --> 01:39:15,900
¿Cómo hacemos para calcular la probabilidad de obtener el estado, no sé, el que quieran, el 1 1 0?

824
01:39:17,160 --> 01:39:25,880
Tenemos que hacer el módulo de 1, 1, 0 contra "psi" al cuadrado.

825
01:39:26,860 --> 01:39:32,340
Bien, cuando hacen módulo de 1, 1, 0 contra "psi"

826
01:39:33,080 --> 01:39:47,340
esto es igual a 1, 1, 0 contra 1 sobre raíz de 8 por 0, 0, 0, más 0, 1, 0, etcétera.

827
01:39:48,340 --> 01:39:57,660
Ahora ¿qué va a pasar? Tiene que hacer este contra este, este contra este, si tiene que aplicar 1, 1, 0 contra cada uno de los términos de la suma.

828
01:39:58,780 --> 01:40:04,540
¿Qué va a pasar? Yo les dije que dan todo 0 salvo cuando tiene la misma string.

829
01:40:06,000 --> 01:40:12,720
Entonces el único término que va sobrevivir es este, el resto es hace 0 cuando lo multiplique.

830
01:40:15,060 --> 01:40:24,600
¿Y qué coeficiente tiene? 1/8. Entonces, lo que va acá arriba, el p110 es módulo de 1/8,

831
01:40:24,660 --> 01:40:37,380
8 al cuadrado y es un octavo, entonces la probabilidad, volviendo, la probabilidad de

832
01:40:37,580 --> 01:40:44,640
detectar alguno de los resultados estos va a ser un octavo, si estaban con 3 qubits y

833
01:40:44,640 --> 01:40:53,180
va a ser un tercio así, con dios qubits un medio, y este estado, este truquito de aplicar

834
01:40:53,180 --> 01:41:01,220
a cada uno de los qubits es muy usado en computación cuántica. Bien, y cuando tengan n qubits,

835
01:41:03,320 --> 01:41:14,840
si aplican que esto sería así, ¿no? Esto sería así, tiene el primer qubit, aplican

836
01:41:14,860 --> 01:41:23,880
Javamar, segundo quibir, Javamar, esta toda, hasta el último quibir, esta es la típica,

837
01:41:25,020 --> 01:41:35,520
tanto en cero, empiezan todos en cero y le aplican Javamar a cada uno de ellos, a la salida

838
01:41:35,860 --> 01:41:44,840
tienen este estado acá, que es la superposición con este coeficiente de todas las posibles

839
01:41:45,400 --> 01:41:49,760
combinaciones de bit strings que pueda haber en la base computación, hay 2 a la n

840
01:41:54,880 --> 01:42:01,720
entonces si tienen 3 hay 8 así, si tienen 4 quebis van a haber 16 etcétera, entonces la probabilidad

841
01:42:02,240 --> 01:42:14,820
la probabilidad de obtener una bit string, dado que está en el estado "psi" es igual a 1 sobre 2 a la n

842
01:42:15,340 --> 01:42:22,640
pueden hacer la cuenta para este estado, el estado que es la...

843
01:42:23,200 --> 01:42:24,640
Bueno, se entiende alguna pregunta?

844
01:42:28,800 --> 01:42:35,300
No, por el momento no, si tiene el mismo es uno, si no es cero, directamente listo.

845
01:42:36,320 --> 01:42:37,860
Después ahí estaba todo pulmolchado.

846
01:42:39,120 --> 01:42:43,040
Claro, pero tenés que tener en cuenta el coeficiente que acompaña, porque esté acá,

847
01:42:43,040 --> 01:42:53,500
este bichito para que anoto. Yo lo escribí afuera, ¿no? con este paréntesis, pero esto en realidad

848
01:42:53,780 --> 01:43:01,380
multiplica de este, multiplica de este, multiplica de tantas. Es decir, la probabilidad va a ser

849
01:43:01,400 --> 01:43:02,740
de influyidad por este cosito.

850
01:43:04,800 --> 01:43:08,180
-Bueno, había dicho que SN da lo "cubit", ¿no?

851
01:43:09,440 --> 01:43:14,320
-Sí, acá SN es el número de crédito. Y esto, esta suma se puede escribir y lo vamos

852
01:43:14,320 --> 01:43:24,080
a hacer de forma compacta así. Suma sobre el raíz de 2 al SN de x en 0 a 1 al SN de x.

853
01:43:24,400 --> 01:43:25,480
acá x

854
01:43:30,800 --> 01:43:32,700
x va a ser una bit string

855
01:43:35,320 --> 01:43:38,780
que es 0 1 1 0 lo que sea 0 1

856
01:43:39,000 --> 01:43:42,540
entiendes? 0 1 al n

857
01:43:45,160 --> 01:43:53,480
es igual al conjunto 0 1 por 0 1 por 0 1

858
01:43:54,000 --> 01:44:01,460
n veces por 0,1. Básicamente es el conjunto de todas las posibles cadenas de 0 y 1 del

859
01:44:01,600 --> 01:44:08,940
arbol, hay dos a la n cadenas. Entonces acá sumo sobre todas las bit strings

860
01:44:09,220 --> 01:44:15,580
posibles o las cadenas de bit posibles donde x va rangando entre el 0 y 1 al arbol.

861
01:44:15,880 --> 01:44:16,740
¿Se entiende la anotación?

862
01:44:19,840 --> 01:44:20,660
-Sí. -Sí.

863
01:44:22,640 --> 01:44:24,580
Esto es lo mismo que hay acá, ¿sí?

864
01:44:25,340 --> 01:44:27,680
Lo mismo que pongo en el lado izquierdo de la ecuación.

865
01:44:28,110 --> 01:44:32,360
Es una forma compacta de describir lo que hay en el lado izquierdo.

866
01:44:32,360 --> 01:44:40,000
Es sumar todas las posibles combinaciones del 0 y 1 que hay allá de largo N.

867
01:44:43,220 --> 01:44:46,320
¿Y cuántas listas hay en 0 y 1? Dos ala en el listas.

868
01:44:46,640 --> 01:44:50,480
tienen 2 queubis en 4 listas y 3 queubis en 8, así sigue.

869
01:44:50,840 --> 01:44:51,720
Lo salen bien.

870
01:44:53,040 --> 01:44:55,920
Entonces, bueno, podemos armar gatos de Jodrk cada vez más

871
01:44:56,000 --> 01:44:58,140
grandes, que es esto que les estaba diciendo acá.

872
01:45:00,320 --> 01:45:02,420
Y la otra cosa relevante es que, miren,

873
01:45:04,580 --> 01:45:08,180
si se lo aplico al 0, 0, 0, obtengo esto de acá.

874
01:45:10,180 --> 01:45:10,660
Esto.

875
01:45:12,240 --> 01:45:14,300
Esto es cuando lo aplico al 0, 0, 0.

876
01:45:14,720 --> 01:45:21,960
Ahora, ¿Qué pasa si en vez de inicializar los qubits en 0, 0, 0, los inicio en otro estado,

877
01:45:22,360 --> 01:45:27,000
que es yo del 0, 1, 0, 1, 1, 1, o decir 1 que no sea el que tiene todos 0s.

878
01:45:27,640 --> 01:45:32,720
Bueno, este puede ser un ejercicio más difícil, pero se puede hacer, está creado en el Niel

879
01:45:32,760 --> 01:45:39,880
Selicone, les queda como ejercicio hacerlo, se aplican hadamard a todos los qubits,

880
01:45:40,520 --> 01:45:44,320
ahora con los kutsin inicializados en un estado que no es el que tiene todos

881
01:45:44,580 --> 01:45:50,120
ceros, les queda muy parecido el caso anterior, les queda muy parecido,

882
01:45:54,680 --> 01:45:59,660
este era el caso anterior y el caso nuevo es muy parecido, tiene el mismo

883
01:45:59,700 --> 01:46:07,520
coeficiente todo, pero lo que cambió es que acá aparece una fase, un -1 a la

884
01:46:07,520 --> 01:46:16,920
x por y, donde y es la primera bitstring, la primera cadena de c o c 1 y x tiene que ir variando por

885
01:46:17,120 --> 01:46:29,700
todas las, entonces ¿y qué quiere decir x por y acá? por ejemplo si x es 0 0 1 1 y es 1 1 1 1 x por y

886
01:46:29,700 --> 01:46:38,800
es como el producto escalar, este por este, cero por este más, cero por uno más, uno por uno más,

887
01:46:39,400 --> 01:46:41,820
uno por uno, ¿sí? ¿Se entiende?

888
01:46:45,260 --> 01:46:53,360
Y atención, esto está hecho módulo 2, porque esto es de cero más cero más uno más uno,

889
01:46:53,400 --> 01:47:04,700
pero 1+1 m/2 es 1, recuerden, importantísimo, suma m/2 que típicamente esta apuesta si,

890
01:47:04,900 --> 01:47:23,380
en los libros de compilación cuántica es 0+0=0, 0+1=1, 1+0=1 y 1+1=0, yo que puse

891
01:47:23,380 --> 01:47:29,340
uno lo puse mal, acá va un CELA, me confundan. Ok, esta es la suma módula 2.

892
01:47:32,180 --> 01:47:33,460
¿Entiendes esto? Preguntas.

893
01:47:37,600 --> 01:47:38,820
No, ninguna por ahora.

894
01:47:38,860 --> 01:47:43,740
Bueno, esto recuerdenlo. Ok, nada.

895
01:47:44,700 --> 01:47:46,920
Entiendo que por ahí les fue llegada para hacer difícil esto,

896
01:47:48,260 --> 01:47:52,380
pero tengan los mentes hasta el positivo, porque estas dos fórmulas

897
01:47:52,380 --> 01:48:01,820
fórmulas van a aparecer más adelante y si las mastican ahora después le va a resultar más fácil entender lo que va a venir en las futuras clases.

898
01:48:01,980 --> 01:48:13,800
¿Está bien? Bien, seguimos. Ven acá puse el ejemplo de 2 qubits. Bueno, y así siguiendo.

899
01:48:15,500 --> 01:48:23,820
y ven que acá calculé por ejemplo para 2 qubits este producto escalar, la probabilidad de obtener el 1,0

900
01:48:25,240 --> 01:48:32,880
como hice esto? bueno tuve que hacer el producto escalar entre 1 y 5, lo hago acá, tengo que hacer

901
01:48:36,780 --> 01:48:51,680
1 0 contra 1, se le da raíz de 4 por 0 0 0 1 más 1 0 más 1 1, bien cuando hay producto

902
01:48:51,860 --> 01:49:07,280
1 0 por 0 0 da 0, 0 más 1 0 por 0 1 da 0 más ahora sí 1 0 por 1 0 da 1 pero 1 estaba acompañado

903
01:49:07,280 --> 01:49:17,380
el 1 a la raíz de 4 y por último 1 0 por 1 1 a la 0 entonces esto da 1 a la raíz de 4

904
01:49:17,380 --> 01:49:23,380
cuando va el módulo del cuadrado de uno a se doro de 4 me queda 1/4 y esto explica esta

905
01:49:23,460 --> 01:49:30,900
fórmula de acá ¿si? entonces este estado es tal que la probabilidad de observar la bit

906
01:49:31,020 --> 01:49:37,560
string 1 0 dado que el sistema está preparado en este estado es 1/4, es como un dado con

907
01:49:37,580 --> 01:49:50,940
cuatro caras. Bien, y lo mismo si tienen ocho quíbes. Bueno, ahora vamos a ver un

908
01:49:51,000 --> 01:49:55,560
algoritmo, un ejemplo de algoritmo cuántico que es de juguete, al final de la

909
01:49:55,680 --> 01:50:01,460
clase va a quedar claro por qué es de juguete, pero sirve para explicar por qué,

910
01:50:01,460 --> 01:50:07,440
¿Por qué uno podría esperar que la computación cuántica del lugar algún

911
01:50:07,680 --> 01:50:08,480
tipo de ventaja?

912
01:50:14,400 --> 01:50:19,380
Acá la ventaja se ve respecto de una computadora clásica

913
01:50:21,740 --> 01:50:24,500
determinista. Ahora vamos a tratar de ver qué quiere decir eso.

914
01:50:26,620 --> 01:50:34,080
Bien, para entender esto es muy importante entender el problema, si no entienden el problema que se está

915
01:50:34,100 --> 01:50:40,380
resolviendo no van a entender el algoritmo. El problema es raro, es un problema que no tiene una

916
01:50:40,440 --> 01:50:47,220
aplicación práctica directa, es como una especie de problema de juguete, pero bueno una función

917
01:50:47,840 --> 01:50:58,320
que haga el 0 1 a la n, acuérdense el 0 1 a la n serían las cadenas de 0 y 1 de largo n,

918
01:51:00,480 --> 01:51:08,380
vimos que para 3 que hubiera salida 8, pero bueno igual nada esto es una función clásica del 0 1 a la n

919
01:51:08,380 --> 01:51:20,800
el 0 1, es constante si f(x) es 0 para todo x o f(x) es igual a 1 para todo x, y es balanceada

920
01:51:21,680 --> 01:51:32,540
si la mitad de las veces da 0 y la mitad de las veces da 1, por ejemplo, vamos al caso

921
01:51:32,580 --> 01:51:43,460
más fácil, una F que va del 0 1 al 0 1, bueno, supongan que agarran la que a 0 lo

922
01:51:43,520 --> 01:51:49,340
manda a 1 y a 1 lo manda al 0, esta es balanceada porque la mitad de las veces da 1 y la mitad

923
01:51:49,340 --> 01:51:54,180
de las veces da 0, acá hay dos veces, hay dos posibilidades, 0 y 1, bueno, cuando le

924
01:51:54,180 --> 01:52:03,100
le valúo en 0 da 1, cuando le volúo en 1 da 0, entonces es balanceada, esta otra es constante,

925
01:52:05,420 --> 01:52:11,380
¿por qué? porque siempre vale 0, constante es que siempre toma el mismo valor, entonces

926
01:52:11,500 --> 01:52:22,740
esta vale siempre 0, esta otra instancia es balanceada, porque al 0 le manda al 0 y al

927
01:52:22,740 --> 01:52:26,640
lo manda a uno, bueno cumple que la mitad de las veces a 0 y la mitad de las veces a 1

928
01:52:27,160 --> 01:52:32,780
y por último, esta de acá es constante, porque a todo lo manda a uno.

929
01:52:40,760 --> 01:52:42,640
Al final era malísimo este cosa.

930
01:52:44,700 --> 01:52:46,760
En otro día lo probé y me andaba fenómeno ahí.

931
01:52:48,360 --> 01:52:49,200
Bueno, poniérala.

932
01:52:50,900 --> 01:52:51,740
No sé qué pasa.

933
01:52:55,840 --> 01:52:57,220
Bueno, vamos al Whiteboard.

934
01:53:00,790 --> 01:53:04,620
Por ahí lo que me está pasando es que Internet no está andando muy bien.

935
01:53:26,199 --> 01:53:31,740
Lo de escribir acá. Supongo que tienen una de ocho.

936
01:53:38,200 --> 01:53:41,780
porque esta era el caso más sencillo o una de cuatro supongamos que tengo

937
01:53:43,460 --> 01:53:44,400
un modo que tienen

938
01:53:46,500 --> 01:53:49,900
00, 01, 10 y 11

939
01:53:51,360 --> 01:53:54,000
bueno voy poniendo ejemplos

940
01:53:56,600 --> 01:54:02,940
vamos a poner f1, f2, f3 y f4

941
01:54:02,940 --> 01:54:08,520
Supongo que la F1 al 0,0 lo manda al 0, al 0,1 lo manda al 0, al 1,0,0

942
01:54:09,280 --> 01:54:12,060
Bueno, esta es constante, constante

943
01:54:14,240 --> 01:54:20,020
Pero si hago, no sé, a los dos primeros los mando al 0, de los últimos al 1, es balanceada

944
01:54:21,100 --> 01:54:23,320
Porque la mitad fuera al 0 y la mitad fuera al 1

945
01:54:25,400 --> 01:54:28,280
Y la F3 podría ser 1, 1, 1, 1, ¿sí?

946
01:54:28,500 --> 01:54:36,940
esa es constante también y qué pasa si hago no sé 0 1 1 1 al 0 al 0 lo mando al 0 al 0 1

947
01:54:37,000 --> 01:54:45,320
lo mando al 1 al 1 0 al 1 y al 1 1 1 esta no es ni constante ni balanceada constante no es porque

948
01:54:45,320 --> 01:54:51,020
no vale ni siempre 0 ni siempre 1 a veces vale 0 a veces vale 1 pero no es balanceada porque

949
01:54:52,500 --> 01:54:57,860
tres veces vale 1 y una vez vale 0 no es la mitad de veces 0 y la mitad de la vez es 1 se entiende

950
01:55:02,680 --> 01:55:07,460
entonces balanceada quiere decir que la mitad de los inputs vale 0 y la otra mitad vale 1

951
01:55:08,440 --> 01:55:15,040
fíjense que siempre hay un número par de inputs porque hay 2 al an inputs y no sabe el spar

952
01:55:15,400 --> 01:55:24,179
se hace en 2 al an y sobre 2 es 2 al an -1 que es par, si están en 4 inputs y están en 2 a la 2

953
01:55:24,180 --> 01:55:31,420
los que en la mitad es 2 y si está en 8 la mitad es 4, bien.

954
01:55:35,020 --> 01:55:40,920
Bien, entonces esa es la noción de constante y balanceada, acá puse, bueno, ahí las cuatro

955
01:55:41,040 --> 01:55:49,740
funciones, entonces primero lo vamos a resolver así, hay dos clases, C1 y C y B, la de las

956
01:55:49,740 --> 01:55:58,680
si la de las balanceadas. Entonces, en objetivo, el planteamiento del problema es que hay que

957
01:55:58,780 --> 01:56:05,320
determinar si F es constante o balanceada bajo la premisa de que pertenece a alguna de las dos

958
01:56:05,480 --> 01:56:14,380
clases. Para el caso este es trivial porque o es constante o no es trivial pero o es constante

959
01:56:14,380 --> 01:56:21,600
es balanceada pero si le pongo bit strings más largas a los inputs hay algunas que

960
01:56:21,600 --> 01:56:29,000
no son ni constantes ni balanceadas como les mostré recién. Entonces acá no es

961
01:56:29,000 --> 01:56:36,600
que están determinando cualquier función sino el problema asume que el que va a

962
01:56:36,630 --> 01:56:44,360
tener que resolver el problema tiene la certeza de que la función desconocida es

963
01:56:44,360 --> 01:56:47,220
o constante valenciada, no sabemos qué función es,

964
01:56:48,880 --> 01:56:54,020
tampoco sabemos si es constante valenciada pero sabemos con certeza que es constante o que es valenciada.

965
01:56:55,380 --> 01:56:57,860
Entonces el objetivo es determinar

966
01:56:59,580 --> 01:57:00,900
a qué clase pertence a la función.

967
01:57:03,640 --> 01:57:07,740
Pero hay que hacernos haciendo la menor cantidad de

968
01:57:07,760 --> 01:57:09,100
evaluaciones posibles de la función.

969
01:57:15,480 --> 01:57:23,880
a ver, esto, ver si me deja volver...

970
01:57:27,320 --> 01:57:33,460
es muy malo este problema, pudo creer que esto será malísimo, vale.

971
01:57:42,260 --> 01:57:44,380
¿Cómo sería resolver este problema clásicamente?

972
01:57:45,240 --> 01:57:50,380
¿Adiós me podría decir cuántos pasos requiere resolver este problema con algo alismo clásico?

973
01:57:54,520 --> 01:57:56,780
Esto está descartado completamente.

974
01:58:05,240 --> 01:58:06,000
¿Alguien se anima?

975
01:58:06,940 --> 01:58:08,580
A ver, yo diría que...

976
01:58:09,600 --> 01:58:11,080
midiendo cada uno de los f's, ¿no?

977
01:58:21,860 --> 01:58:23,380
¿Cómo cada uno de los hechos?

978
01:58:25,400 --> 01:58:28,920
Sabes que te da un número.

979
01:58:30,840 --> 01:58:31,900
¿Ves si he balanceado o no?

980
01:58:32,370 --> 01:58:33,320
¿Lo comparas con el otro?

981
01:58:36,480 --> 01:58:37,480
¿Cómo a poco a poco?

982
01:58:38,240 --> 01:58:39,580
no pasa nada.

983
01:58:52,720 --> 01:58:56,440
No, mira, tenés que hacer una cuenta para resolverlo.

984
01:58:56,880 --> 01:58:57,600
vamos a volver acá nada

985
01:59:03,880 --> 01:59:07,740
pensemos suponerte que vos tenés la F

986
01:59:10,780 --> 01:59:12,240
lo voy a escribir acá

987
01:59:17,500 --> 01:59:20,380
vos en este caso tenés

988
01:59:22,880 --> 01:59:26,160
Espera, vamos a volver a la otra diapositiva.

989
01:59:27,000 --> 01:59:34,120
Acá, a vos te dan una función de estas, en el caso 01 al 01.

990
01:59:34,590 --> 01:59:39,840
Tenés que determinar si la función es constante o balanceada.

991
01:59:41,139 --> 01:59:46,740
Entonces, vas a calcular cuántos pasos tengo que dar para resolverlo

992
01:59:47,800 --> 01:59:53,840
suponerte que hago una evaluación en la primera ronda llamo la función una vez

993
01:59:54,160 --> 02:00:04,080
suponerte que me da algo f0 y me da 1, a partir de esta evaluación vos

994
02:00:04,160 --> 02:00:14,199
podés concluir si es contante o balanceada? no porque tenés este caso este caso

995
02:00:14,200 --> 02:00:18,160
este caso o este caso, es alguna de estas cuatro, pero esta información no te

996
02:00:18,200 --> 02:00:22,560
permite dirimir si vas a ser constante o balanceada, ¿por qué? porque en la próxima

997
02:00:22,720 --> 02:00:27,620
evaluación f1 podría ser o 0 o 1, ¿entendés?

998
02:00:29,720 --> 02:00:33,220
entonces en este caso o vola tenés que evaluar dos veces a la función, ¿tás

999
02:00:33,260 --> 02:00:39,500
acuerdo? sí, sí o sí, si no no te alcanza para resolver el problema, bien,

1000
02:00:40,920 --> 02:00:45,640
bien ahora qué pasa para la que tiene cuchada para para la que tiene tres no

1001
02:00:45,740 --> 02:00:52,260
para que tiene dos no dos si tengo los inputs son

1002
02:00:57,880 --> 02:01:06,700
los inputs son 0 0 0 1 1 0 y 1 1 acá también yo estoy seguro de que la f es o

1003
02:01:06,700 --> 02:01:10,900
constante o balanceada pero no sé a cuál de las dos clases pertan a ese. Entonces bueno,

1004
02:01:12,980 --> 02:01:18,860
consulto al agráculo una vez, en la primera vuelta hago f00, me da, no sé, supongo que

1005
02:01:18,880 --> 02:01:29,820
me da 1, ¿sí? ¿Me alcanza para adimir si f es constante o balanceada? No. Bueno, consulto

1006
02:01:29,820 --> 02:01:40,800
de vuelta, 2, AF01, suponente que me da a 0, bueno ahí que me pasó, ahí puedo concluir

1007
02:01:40,880 --> 02:01:50,500
que es balanceada o no, porque no es constante, y porque no es constante, si fuera constante

1008
02:01:50,720 --> 02:01:52,800
tendría que haber dado uno de vuelta, ¿entendés?

1009
02:01:55,700 --> 02:01:58,780
Pero, lo gananciada, una a la dos, que se dice, o si?

1010
02:01:59,820 --> 02:02:03,440
Claro, yo estoy bajo la hipótesis de que es una de las dos.

1011
02:02:03,860 --> 02:02:04,160
Atención.

1012
02:02:04,960 --> 02:02:07,980
Ahora, suponente que me daba uno de vuelta, ¿entendés?

1013
02:02:08,240 --> 02:02:08,760
Me daba uno.

1014
02:02:09,960 --> 02:02:13,320
Si me daba uno, ahora con esto no me alcanza,

1015
02:02:13,420 --> 02:02:17,360
porque podría ser que en las otras dos entradas,

1016
02:02:17,620 --> 02:02:21,720
en 1, 0 y en 1, 1, me dé 1 y 1 o no, que me dé 0,

1017
02:02:21,920 --> 02:02:22,480
¿entendés?

1018
02:02:23,100 --> 02:02:23,640
Yo no lo sé.

1019
02:02:24,080 --> 02:02:26,560
Con estas dos primeras evaluaciones no me alcanza.

1020
02:02:26,700 --> 02:02:27,040
¿Me seguís?

1021
02:02:28,380 --> 02:02:28,580
Claro.

1022
02:02:33,000 --> 02:02:35,640
Entonces yo necesito una evaluación más.

1023
02:02:35,910 --> 02:02:36,340
¿Me entendás?

1024
02:02:37,070 --> 02:02:39,120
Yo necesito fijarme cuánto vale, por ejemplo,

1025
02:02:39,240 --> 02:02:39,540
F10.

1026
02:02:40,280 --> 02:02:41,920
Si vale 0, ahí ya concluyo.

1027
02:02:42,060 --> 02:02:44,420
Ya estoy seguro de que es balanceada.

1028
02:02:44,470 --> 02:02:46,420
Y si vale 1, ya estoy seguro de que era constante.

1029
02:02:47,280 --> 02:02:47,560
Sigo.

1030
02:02:47,820 --> 02:02:48,240
Atención.

1031
02:02:49,180 --> 02:02:51,080
Abamos la de 3 a riesgo de cansar.

1032
02:02:56,540 --> 02:03:10,320
Suponente que tengo 0,000, 0100, 0,01, 1,010, 0110, 1,010, 1,110 y "1 1 1", son 8, no?

1033
02:03:10,840 --> 02:03:25,540
bueno, en la primera evaluación hago f(0,0) y me da 1, si en la segunda evaluación el f(1,0) me da 0, ya está, ya concluyo que es balanceado

1034
02:03:25,740 --> 02:03:26,580
pero me podría dar uno.

1035
02:03:27,980 --> 02:03:29,660
Y en la tercera evaluación también.

1036
02:03:32,980 --> 02:03:33,720
También me podría dar.

1037
02:03:33,800 --> 02:03:35,900
Y en la cuarta evaluación, también,

1038
02:03:36,020 --> 02:03:37,120
si tengo mala suerte, ¿no?

1039
02:03:37,280 --> 02:03:38,020
Tengo mala suerte.

1040
02:03:38,740 --> 02:03:39,340
Me vuelvo a dar uno.

1041
02:03:39,840 --> 02:03:40,920
Fijate lo que me está pasando.

1042
02:03:41,740 --> 02:03:44,940
Con estas 4, que es la mitad, acá tengo 8, ¿no?

1043
02:03:45,860 --> 02:03:46,360
Tengo 8.

1044
02:03:47,180 --> 02:03:50,360
Evaluvo las primeras 4 y en todas me veo uno.

1045
02:03:50,760 --> 02:03:55,720
Ahora, en la quinta evaluación, ¿quién me garantiza que a partir

1046
02:03:55,720 --> 02:04:02,560
yo sé hasta ahora puedo garantizar que va a dar 0 o 1 no no lo sé entendés

1047
02:04:06,720 --> 02:04:11,500
entonces entonces cuando le valúe de vuelta me va a dar 1 o 0 bueno suponerte

1048
02:04:11,500 --> 02:04:15,920
que 0 1 1 me dio 1 ahí concluyo que es constante si me va a hacer o concluyo que

1049
02:04:15,940 --> 02:04:22,360
vale así entonces la monareja es esta para el caso n vas a tener que hacer la

1050
02:04:22,360 --> 02:04:28,100
mitad de las evaluaciones, vos tenés dos a la n posibilidades, vas a ver la mitad de

1051
02:04:28,160 --> 02:04:34,620
las evaluaciones más uno, ¿entendés? Este número de pasos es el que te garantiza resolver

1052
02:04:34,740 --> 02:04:37,100
con certeza absoluta el problema, ¿me seguirán?

1053
02:04:38,840 --> 02:04:44,200
No, no entendí el por qué dividió dos, yo pensé que era...

1054
02:04:44,320 --> 02:04:52,700
por esto, por esto, por esto, mira, tenés la bada vuelta, es una goma esto pero es importante

1055
02:04:52,840 --> 02:04:53,300
entenderlo, ¿no?

1056
02:04:53,620 --> 02:04:59,920
Yo entendí el 2n + 1, yo lo desgasta ahí pero no entendí, a la 2.

1057
02:04:59,920 --> 02:05:04,780
Sí, sí, sí, para, 1, 0, 1, 0, 1, 1, 1, 1, 1, 1.

1058
02:05:06,020 --> 02:05:08,640
Viscante que si yo valgo la mitad de las veces, ¿no?

1059
02:05:09,760 --> 02:05:14,980
no me alcanza habíamos dicho, toque evaluar la mitad más uno de las veces, ¿entendés?

1060
02:05:15,520 --> 02:05:15,640
si

1061
02:05:16,600 --> 02:05:27,900
bueno este es el caso n igual a 3 que sería 2 al cubo que es 8, ¿entendés? 3, 8

1062
02:05:30,200 --> 02:05:39,960
si pongo 2 a la n, ¿cuál es la mitad de 2 a la n? 2, 2 a la n dividido 2, ¿entendés?

1063
02:05:40,420 --> 02:05:46,740
Esto yo tengo que hacer, 2 a la n dividido 2 y con esa lo me alcanzan más 1 evaluaciones,

1064
02:05:46,920 --> 02:05:47,240
¿entendés?

1065
02:05:48,100 --> 02:05:48,800
Soy ahí, no entendí.

1066
02:05:50,140 --> 02:05:57,700
Este es el número de pasos que el algoritmo clásico debe dar, clásico determinista en

1067
02:05:57,700 --> 02:06:02,860
en el sentido de que clásico con certeza absoluta, que te permite resolver con certeza absoluta el problema,

1068
02:06:04,360 --> 02:06:07,980
2 a la n sobre 2 más 1. Y este número es exponencial.

1069
02:06:10,020 --> 02:06:13,740
¿Por qué esto crece exponencialmente con n? ¿Se entienden?

1070
02:06:15,920 --> 02:06:24,020
Bueno, hay una pregunta. Entonces, acá la redice en este caso que la complejidad oracular de este problema es exponencial.

1071
02:06:26,260 --> 02:06:31,720
este número fíjate que es 2 a la n-1, 2 a n sobre 2, eso es a n-1 más 1.

1072
02:06:32,380 --> 02:06:39,420
Entonces la complejidad oracular del caso clásico es exponencial, ¿por qué?

1073
02:06:40,080 --> 02:06:47,980
Porque para resolverlo tenés que hacer, tenés que hacer la mitad de las veces, la

1074
02:06:48,020 --> 02:06:54,821
pregunta al oráculo, la mitad más 1 y eso es 2 a la n sobre 2 más 1 y ese es un

1075
02:06:54,820 --> 02:07:01,240
número exponencial porque por qué no sale a la input son muchos se entiende entonces esto se

1076
02:07:01,280 --> 02:07:07,660
vuelve rápidamente intratable si pones un en muy grande se te sale de escalas el problema

1077
02:07:07,980 --> 02:07:17,980
me entendés aunque no se me ocurre cómo lo mueve cuánticamente como como sería bueno

1078
02:07:19,160 --> 02:07:25,680
matemática cuántica, qué sé yo, nada, ahora vemos, pero bueno, esto es el primer mensaje,

1079
02:07:26,090 --> 02:07:29,700
es un problema ficticio, a nadie le importa resolver esto, pero importa, es un problema

1080
02:07:29,780 --> 02:07:35,460
matemático que la complejidad oracular del algoritmo clásico es exponencial.

1081
02:07:37,960 --> 02:07:45,541
Ahora vamos a ver cómo resolverlo cuanticamente. Entonces, da una F que va del 0,1 al A en el

1082
02:07:45,540 --> 02:07:50,200
01 queremos determinar si es con tanto balanceada haciendo la menor cantidad de

1083
02:07:50,240 --> 02:07:54,960
evaluaciones posibles de la función, es decir, consultando un oráculo que nos

1084
02:07:55,000 --> 02:07:57,880
puede decir cuánto vale la F en un imputado.

1085
02:07:58,380 --> 02:08:02,640
Esto del oráculo lo pueden pensar como cuando tienen que usar una instancia de

1086
02:08:02,680 --> 02:08:09,880
cómputo en la nube, por ejemplo, de AWS. Si cada vez que tiene un algoritmo, que

1087
02:08:09,920 --> 02:08:14,821
cada vez que tiene que correr una subroutine, hay que gastar plata, entonces

1088
02:08:14,820 --> 02:08:19,920
ustedes quieren diseñar el algoritmo o su resolución de problemas al cliente de

1089
02:08:20,040 --> 02:08:25,200
forma tal de gastar la menor cantidad de plata posible. Entonces esa subroutina que cuesta

1090
02:08:25,240 --> 02:08:30,600
plata la quieren correr la menor cantidad de veces posible. Se entiende, acá la subroutina

1091
02:08:30,710 --> 02:08:37,180
sería consulta al oráculo. Es un problema que les puede aparecer naturalmente en su

1092
02:08:37,320 --> 02:08:43,461
práctica de programadores. Ustedes tienen que para resolver cierta tarea cada tanto

1093
02:08:44,540 --> 02:08:50,700
hay que usar una instancia de cómputo que cuesta dinero. Entonces, ustedes quieren diseñar su

1094
02:08:50,740 --> 02:08:58,480
solución para el cliente de forma tal de que esa consulta la "a" la menor cantidad de veces.

1095
02:09:00,420 --> 02:09:07,821
Lo digo esto para, por si ayuda a fijar un poco de líneas acá, el gasto estaría, se pongan que cada

1096
02:09:07,820 --> 02:09:13,380
ves que evaluan la F y consultan el agráculo y le sale 10 dólares, bueno, 2 al n le saldrá

1097
02:09:13,440 --> 02:09:24,220
infinito, es un algoritmo empobrecedor. Bien, entonces vamos a ver la resolución cuántica,

1098
02:09:25,120 --> 02:09:31,200
entonces tenemos F que va del 0,1 al 0,1, vamos a hacer primero el caso fácil, el caso este,

1099
02:09:33,140 --> 02:09:40,120
Las f son así, estas son las cuatro f posibles, entonces vamos a hacer un algoritmo cuántico que

1100
02:09:40,180 --> 02:09:44,220
resuelve para este caso y después lo vamos a hacer para todo vener, para el nervio vital.

1101
02:09:44,950 --> 02:09:52,120
Bien, entonces inicializamos a la computadora cuántica en 0,1. ¿Cómo se hace eso?

1102
02:09:53,220 --> 02:10:06,740
fácil, hacemos X, se acuerdan que la compuerta X, si esta está en 0 y esta está en 0, esto lo hace ir a parar al 0 1

1103
02:10:07,320 --> 02:10:12,500
aplicamos la compuerta X al segundo cube, entonces el primer paso es inicializar la computadora

1104
02:10:12,600 --> 02:10:23,200
cuáltrica en 0 1, el segundo paso es aplicarle Hadamard a todos, entonces el próximo paso hacemos

1105
02:10:23,200 --> 02:10:32,220
"jadamar" que es esto de acá, "jadamar" "jadamar" 0,1. Bueno, cuando hacen esto les queda "jadamar" por 0

1106
02:10:32,270 --> 02:10:42,540
que es 0 + 1 / 2 y "jadamar" por 1 que era 0 - 1 / 2. Entonces sale un factor ahí, 1 / 2 al cuadrado

1107
02:10:44,200 --> 02:10:49,280
que es un medio pero no importa, entonces lo vamos a arrastrar. Y cuando hacen acá el producto

1108
02:10:49,880 --> 02:10:56,080
todos contra todos, cuando hacen este por este, este por este, este por este, este por este,

1109
02:10:56,220 --> 02:11:05,080
les queda esta superposición de acá que tiene como coeficiente cada uno un cuarto, sí, un cuarto.

1110
02:11:12,600 --> 02:11:13,640
¿No salió un medio?

1111
02:11:16,360 --> 02:11:18,200
Un medio, perdón, me confundí.

1112
02:11:19,180 --> 02:11:20,420
Me confundí. Un medio.

1113
02:11:20,920 --> 02:11:21,060
Gracias.

1114
02:11:22,000 --> 02:11:23,760
Qué bueno, qué bueno, gracias gente atenta.

1115
02:11:24,920 --> 02:11:25,880
Ayuda mucho, gracias.

1116
02:11:26,680 --> 02:11:26,740
Bien.

1117
02:11:28,160 --> 02:11:29,080
Entonces, este de acá,

1118
02:11:29,980 --> 02:11:32,600
este de acá es el segundo paso del algoritmo.

1119
02:11:32,720 --> 02:11:34,840
Es el estado de la computadora cuántica.

1120
02:11:37,460 --> 02:11:38,580
Aplicada primero X.

1121
02:11:43,300 --> 02:11:52,160
y después "Hamard" y "Habamard". Este de acá, recuerden no bien, este es este de la

1122
02:11:52,260 --> 02:12:00,540
otra de la positiva, el que yo les dije antes que van como ejercicio y recuerden, era el

1123
02:12:01,660 --> 02:12:07,600
cómo cambiaba la cosa cuando el input era, no eran todos ceros, bueno acá el input era

1124
02:12:07,600 --> 02:12:14,960
el "i" en el ejemplo que estamos viendo ahora, el "i"

1125
02:12:20,400 --> 02:12:25,100
el "i" era 0,1, entonces este

1126
02:12:25,260 --> 02:12:29,440
cosa de acá lo que hace es algunos términos de la sumatoria le sacré un

1127
02:12:29,640 --> 02:12:35,100
menos y es lo que estamos observando acá abajo

1128
02:12:41,360 --> 02:12:46,620
esto, algunos términos de la sumatoria me quedaron con un menos y ese es el -1 al x

1129
02:12:46,720 --> 02:12:52,260
por y que estábamos, por lo que a lo pueden hacer directamente, hacer la cuenta en edad.

1130
02:12:53,600 --> 02:12:58,240
Bien, entonces este es el segundo paso, acá está el circuito, este es el gráfico del circuito,

1131
02:12:59,139 --> 02:13:15,740
Entonces, primero aplico "x" al primer qubit y después le aplico "jadamard" a cada uno de los qubits y luego puede aplicar acto seguido el oráculo, que va a ser la implementación cuántica de la "f" clásica.

1132
02:13:16,840 --> 02:13:28,220
es decir, el oráculo va a ser una compuerta lógica cuántica que lo que hace es darme los inputs, los outputs de cada evaluación de la función que yo le pido.

1133
02:13:28,450 --> 02:13:33,660
Si yo le pido "dame cuánto vale f0" me lo va a decir, esa es la idea.

1134
02:13:37,420 --> 02:13:42,360
Bueno, ¿cómo es un oráculo cuántico? Hace esto, hace esto.

1135
02:13:45,260 --> 02:13:52,660
Si de acá, este sería el oráculo, el U, U sub F, lo escribo más grande acá.

1136
02:13:53,600 --> 02:13:58,080
Sería una matriz unitaria, una transformación inial, que lo que hace es,

1137
02:13:58,320 --> 02:14:06,040
acá input me lo manda a, al primero lo deje igual, tengo x y al primero lo deje igual,

1138
02:14:07,200 --> 02:14:12,160
y al segundo hace la suma módulo 2, recuerden que este, este coso era

1139
02:14:12,960 --> 02:14:24,400
0 + 1, 1 + 0, 1 + 0, 0 y 1 + 1, 0.

1140
02:14:25,600 --> 02:14:26,780
Esto es suma módulo 2.

1141
02:14:28,780 --> 02:14:34,780
Y al segundo qubits lo dejan en el estado y suma módulo 2 f(x).

1142
02:14:35,160 --> 02:14:39,400
Esta es el efecto de la UF.

1143
02:14:41,180 --> 02:14:45,200
Acá a la UF la vamos a tomar como una caja negra.

1144
02:14:45,440 --> 02:14:47,480
No vamos a explicar su síntesis.

1145
02:14:47,660 --> 02:14:49,440
La vez que viene, nos vamos a discutir un poco.

1146
02:14:51,860 --> 02:14:54,080
Pero por ahora nos viene regalada.

1147
02:14:54,260 --> 02:14:57,280
Alguien se tomó el trabajo de armar una comporta lógica

1148
02:14:58,680 --> 02:15:01,520
que dada a la F, hace esto de acá.

1149
02:15:04,700 --> 02:15:05,140
Entonces...

1150
02:15:05,960 --> 02:15:12,600
¿Cómo actúa la F en el 0,0? Bueno, al 0 lo dejo igual y lo mando al 0, suma módulo 2f de 0 y así

1151
02:15:13,040 --> 02:15:21,800
tienen las cuatro posibilidades. Entonces este es el famoso oráculo cuántico que es lo mismo que

1152
02:15:22,060 --> 02:15:28,500
en el caso clásico consultar por una evaluación particular de la F. Entonces lo que queremos

1153
02:15:28,500 --> 02:15:34,540
hacer en el caso cuántico es apelar a la uf la menor cantidad de veces posible.

1154
02:15:38,860 --> 02:15:43,880
Bien, entonces les decía ahora aplican el oráculo y luego vamos a aplicar

1155
02:15:44,400 --> 02:15:47,940
"hama" al primer qubit y vamos a medir el primer qubit.

1156
02:15:49,440 --> 02:15:53,280
Eso es, este es todo el algoritmo, todo el circuito del algoritmo cuántico.

1157
02:15:55,420 --> 02:15:59,240
Bien, entonces este es el paso

1158
02:16:00,780 --> 02:16:06,080
después de aplicar los Habamars y luego aplicamos la UF al paso anterior.

1159
02:16:07,180 --> 02:16:12,940
Recuerden que la UF es lineal, entonces se distribuye en cada uno de los términos de esta suma.

1160
02:16:17,760 --> 02:16:21,080
Acá tienen cuatro términos, entonces cuando aplico la UF a este estado,

1161
02:16:21,740 --> 02:16:24,380
todo es UFD es TUDFD es TUDFD es TUDFD.

1162
02:16:26,120 --> 02:16:30,980
Bien, y ahora aplico lo de la diapositiva anterior, tienen con una tablita de cómo

1163
02:16:31,200 --> 02:16:35,519
actúa UEFA en cada uno de los elementos de la base computacional. Recuerden que una

1164
02:16:35,580 --> 02:16:42,240
transformación lineal quedaba determinada por su acción sobre los elementos de la base

1165
02:16:42,300 --> 02:16:48,840
computacional. Bueno, reemplazo, si voy a la diapositiva anterior, ustedes esto van lo

1166
02:16:48,840 --> 02:16:54,800
de nuevo en sus casas, pero van a la diapositiva anterior y se fijan, UEFA de 0, 0, valía

1167
02:16:54,800 --> 02:16:59,460
esto uf01 valía tanto y así las cuatro evaluaciones

1168
02:17:04,620 --> 02:17:11,519
y lo que voy a hacer ahora fíjense acá viene una cuenta, acá viene por ahí el truquito

1169
02:17:11,580 --> 02:17:18,880
matemático de este algoritmo, a ver cómo puedo hacer, vamos a hacer así, vamos a tratar de escribir acá

1170
02:17:25,140 --> 02:17:32,980
bien, fíjense que acá tienen 0 por esto de acá y tienen 0 por esto de acá, entonces

1171
02:17:33,120 --> 02:17:40,840
este 0 lo podemos sacar factor común, 0 más lo que sea, recuerden la suma módulo 2 será

1172
02:17:40,960 --> 02:17:52,000
0 más y yolá y porque el 0 no cambiaba, entonces este queda f de 0 y este queda uno más f de 0

1173
02:17:52,120 --> 02:17:58,960
como no sé cuánto vale f de 0 no puedo seguir calculando más pero como tengo a todo esto

1174
02:17:59,000 --> 02:18:07,080
multiplicado pues este solo lo saco factor común y pongo este paréntesis y lo mismo hago con

1175
02:18:07,080 --> 02:18:14,080
estos términos, este y este, el 1 aparece en los 2, lo saco factor común y me queda muy

1176
02:18:14,200 --> 02:18:21,540
duplicado por ésta, ¿vale? Bien, esa es la primera cosa y luego, luego vamos a

1177
02:18:21,639 --> 02:18:29,760
realizar estos dos términos por separado, este que es este de acá y este que es este de acá abajo.

1178
02:18:31,740 --> 02:18:36,700
Entonces ahora, como yo lo voy a hacer ahora en la clase pero es probable que no lo entiendan,

1179
02:18:36,719 --> 02:18:45,059
como ejercicio les queda determinar que esto de acá es igual a -1 a la f(0) por

1180
02:18:45,240 --> 02:18:50,860
0 -1, eso se puede hacer por inspección, nosotros no sabemos cuánto vale la f(0)

1181
02:18:53,639 --> 02:19:00,800
no sabemos cuánto vale, no lo sé, sin embargo f(0) o f(0) o f(1)

1182
02:19:02,480 --> 02:19:09,960
no hay otra posibilidad, entonces si f(0), si f(0) es igual a 0, acá obtengo,

1183
02:19:11,801 --> 02:19:20,340
en la primera línea estoy mirando, esto acá estoy mirando, obtengo 0 - 1 + 0 = 1

1184
02:19:21,820 --> 02:19:30,320
y esto coincide con -1 a la 0 por esto y

1185
02:19:30,320 --> 02:19:44,700
y, si es p de cero, he de igual a 1, vuelvo acá, vuelvo esta línea acá, me queda 1 menos

1186
02:19:45,929 --> 02:19:59,120
1 más 1 es 0 y esto es -1 por 0 menos 1, simplemente multipliqué y esto coincide con -1

1187
02:19:59,120 --> 02:20:05,160
a la F de 0, que es 1, entonces vale esta igualdad, les acabo de probar que vale esta,

1188
02:20:05,790 --> 02:20:12,020
les queda como ejercicio ustedes probar que vale esto de abajo, es simplemente convencerse,

1189
02:20:13,140 --> 02:20:20,580
jugar un poco con los posibles valores de la F y convencerse de que esas igualdades son

1190
02:20:20,600 --> 02:20:28,820
ciertas independientemente de cuánto va a ganar a ella. Bien. Y acá aparece el primer

1191
02:20:28,940 --> 02:20:38,060
punto interesante. En este caso cuántico, yo no sé cuánto vale F0 o F1 y no necesito

1192
02:20:38,100 --> 02:20:45,199
saberlo para resolver el problema, como vamos a ver en breve. Bien, sigo. Entonces ahora

1193
02:20:45,200 --> 02:20:51,820
voy a aplicar esto de acá, aplico esto en el C2, les queda como es que a sí se

1194
02:20:51,840 --> 02:20:58,760
usted es mostrar que todo esto es así, aplico ¿no? reemplazo, entonces tengo 0 por -1 al

1195
02:20:58,860 --> 02:21:05,060
F es 0 por 0 -1, 1 por -1 al F es 1 por 0 -1, bien y ahora tengo que hacer

1196
02:21:08,720 --> 02:21:15,180
redistrugio de vuelta si quieren. -Regrupo términos básicamente. -Regrupo estos factores

1197
02:21:15,180 --> 02:21:17,500
y los productos, no se me queda.

1198
02:21:18,680 --> 02:21:19,100
Estoy acá

1199
02:21:27,021 --> 02:21:28,400
y fíjense una cosa.

1200
02:21:36,640 --> 02:21:37,980
Este fíjense una cosa,

1201
02:21:38,400 --> 02:21:39,620
creen que lo tengo que anotar acá.

1202
02:21:41,240 --> 02:21:43,180
Acá me comí una barrito

1203
02:21:44,340 --> 02:21:51,880
y fíjense este término aparece en los dos factores de esta suma, esto y esto,

1204
02:21:53,120 --> 02:21:58,040
entonces a este cosito que se repite lo saco factor común y es este de acá,

1205
02:21:58,640 --> 02:22:09,260
estos dos son este de acá y luego del otro lado me queda -1 al f de 0 por 0 más -1 al

1206
02:22:09,260 --> 02:22:26,080
de f1 más f0. Bien, entonces ahora esto es el cuid 1 y todo esto de acá va en realidad

1207
02:22:26,300 --> 02:22:35,620
si, si y esto de acá refiere al cuid 0, si, entonces ahora nos vamos a enfocar solo en

1208
02:22:35,620 --> 02:22:41,120
el estado del qubitsero, entonces acá hay unos sobre raíz de 2 al cuadrado, unos sobre

1209
02:22:41,220 --> 02:22:46,900
raíz del sal cuadrado es uno sobre raíz de 2 por uno sobre raíz de 2, uno de los unos

1210
02:22:47,100 --> 02:22:53,880
sobre raíz de 2 va acá y el otro se queda acá, si básicamente esto de acá sería el

1211
02:22:53,880 --> 02:23:05,920
estado del covid 0, para descartar un poco y al final del día vuelvo al algoritmo,

1212
02:23:06,020 --> 02:23:11,000
vuelvo al algoritmo, después de que aplico el oráculo,

1213
02:23:14,300 --> 02:23:15,680
decir acá

1214
02:23:21,220 --> 02:23:21,420
pero

1215
02:23:24,280 --> 02:23:32,880
acá, tengo ese estado que les mostré antes y me fijo en el estado del qubit 0

1216
02:23:33,090 --> 02:23:35,080
me olvido momentáneamente el qubit 1

1217
02:23:44,580 --> 02:23:51,280
entonces este era el estado a la salida del oráculo, este de acá el psidos y el

1218
02:23:51,280 --> 02:23:54,860
el simonio es el estado del Qubit 0 a la salida del olácula.

1219
02:23:58,280 --> 02:24:01,140
¿Por qué no incluí el -1 al F de 0?

1220
02:24:01,250 --> 02:24:02,640
Bueno, porque es una fase global.

1221
02:24:03,510 --> 02:24:07,400
Yo les dije antes que este que multiplicaba todo,

1222
02:24:08,240 --> 02:24:09,860
este que multiplicaba todo,

1223
02:24:21,420 --> 02:24:27,120
este que multiplicaba todo como tiene módulo 1 no va a afectar a la probabilidad de transición

1224
02:24:27,390 --> 02:24:33,480
de estado, entonces este lo puedo descartar, lo podría arrastrar si quieren pero no hace falta,

1225
02:24:33,600 --> 02:24:44,680
Bien, entonces me quedó -1, me quedó este estado en el Qubit0 y ahora al Qubit0 le voy a aplicar

1226
02:24:44,840 --> 02:24:50,040
Hadamard de vuelta, aplico Hadamard, bueno, entonces tengo que aplicar Hadamard a cada uno de los términos

1227
02:24:50,040 --> 02:24:56,960
de esta superposición, me queda eso, sigo, esto sería esta última Hadamard de acá,

1228
02:25:02,240 --> 02:25:11,160
a causa, para aplicar "Hammer" uso la regla de "Hammer" de cómo opera "Hammer" sobre el 0 y el 1

1229
02:25:13,320 --> 02:25:19,680
y finalmente el estado que obtengo es este de acá, el "p3" que es este de acá,

1230
02:25:21,320 --> 02:25:31,780
entonces si se fijan me quedan unos coeficientes acá, me quedo algo multiplicando el 0 y algo multiplicando el 1

1231
02:25:32,340 --> 02:25:39,920
entonces si yo ahora voy y mido al qubit 0, perdón, no está en el estado 0, está

1232
02:25:39,960 --> 02:25:47,200
justamente en este estado psi3, si yo ahora mido, entonces voy a obtener con una

1233
02:25:47,260 --> 02:25:51,860
cierta probabilidad 0 y con una cierta probabilidad 1, pero esa probabilidad va a

1234
02:25:51,860 --> 02:25:57,900
estar vinculada a este numerito de acá y a estos coeficientes de acá, recuerden

1235
02:25:57,900 --> 02:26:04,380
esto sería como un alfa por cero más beta por uno, entonces cuando yo mida voy a tener

1236
02:26:05,440 --> 02:26:12,740
módulo alfa al cuadrado, quizás va a ser la probabilidad de obtener cero y módulo de beta al cuadrado,

1237
02:26:13,300 --> 02:26:21,000
que va a ser la probabilidad de obtener uno, entonces me tengo que fijar cuánto vale el módulo

1238
02:26:21,060 --> 02:26:26,460
al cuadrado, esto multiplicado por un medio, para calcular la probabilidad de cero o uno,

1239
02:26:26,500 --> 02:26:28,520
Entonces, esto lo tengo escrito acá.

1240
02:26:31,280 --> 02:26:39,700
Este sería el estado final del Qubit 0, este de acá, el de arriba.

1241
02:26:40,790 --> 02:26:42,260
Me tengo que fijar lo coeficiente.

1242
02:26:43,230 --> 02:26:45,060
Lo voy a escribir acá por las dudas para que no.

1243
02:26:46,560 --> 02:26:47,100
Vamos a hacer así.

1244
02:26:50,880 --> 02:26:56,480
Yo quiero medir ahora, quiero medir y para eso y esa medición

1245
02:26:56,480 --> 02:27:05,180
va a dar 0 o 1 con una cierta probabilidad, bien, entonces a este Psi3 lo

1246
02:27:05,320 --> 02:27:15,100
pensamos como una alfa por 0 más beta por 1, donde alfa es esto de acá por un medio,

1247
02:27:16,240 --> 02:27:24,721
porque en un medio se aplica estos dos factores, entonces el alfa es un medio de

1248
02:27:25,460 --> 02:27:38,080
1 + -1 a la f(1) suma modulo 2 f(0) y el beta es un medio por 1 - -1 a la f(1)

1249
02:27:39,000 --> 02:27:44,140
suma modulo 2 f(0) entonces la probabilidad de obtener 0

1250
02:27:46,080 --> 02:27:51,841
la p(0) es modulo de alfa cuadrado y la p(1) es modulo de alfa cuadrado se entiende

1251
02:27:51,840 --> 02:27:57,260
esto, entiendo que por ahí en las cuentas se están perdiendo, esto también me perdería,

1252
02:28:01,560 --> 02:28:07,880
pero lo importante es que no pierdan de miras cómo yo calculo las probabilidades,

1253
02:28:08,080 --> 02:28:11,940
ustedes después esto lo tienen que poder hacer en lápiz y papel, esa es la idea,

1254
02:28:12,300 --> 02:28:17,420
como ejercicio les queda ir repitiendo uno por uno estos pasos en lápiz y papel.

1255
02:28:24,881 --> 02:28:32,400
Entonces fíjense una cosa, la pregunta sería si f es constante, vamos a calcularlo acá,

1256
02:28:35,800 --> 02:28:44,800
supongamos que f es constante, entonces si f es constante se tiene que convencer que f

1257
02:28:44,800 --> 02:28:52,560
de 0 más f de 1 siempre da 0, ¿por qué? porque si f es constante f de 0 es igual a f de 1, siempre.

1258
02:28:54,080 --> 02:29:06,780
Entonces f(0) suma módulo 2, f(1) da, si vale todo 0 la f o da 0 más 0 o 1 más 1, en caso de que vale todo 1.

1259
02:29:06,940 --> 02:29:12,700
Bueno en cualquiera de los casos esto da 0, porque 0 más 0 módulo 2 es 0 y 1 más 1 módulo 2 es 0.

1260
02:29:13,939 --> 02:29:22,560
siempre que la f sea constante este numerito es 0 y si la f es balanceada f0 + f1 es 1

1261
02:29:23,140 --> 02:29:35,220
¿por qué? porque si es balanceada, es f0 + f1 esto es igual a o 1 + 0 o 0 + 1 en

1262
02:29:35,220 --> 02:29:40,880
cualquiera de los dos casos da 1, ¿Está bien? Entonces ahora vuelvo a lo de arriba.

1263
02:29:45,160 --> 02:29:49,580
Si f es contante, vas a analizar primero el caso f constante.

1264
02:29:54,180 --> 02:29:57,080
Si f es contante, esto vale 0.

1265
02:30:00,760 --> 02:30:12,420
entonces 1 + -1 al a0 es 1 y este término es -1 al a0 = 1, pero 1 -1 es 0, entonces todo este término se va

1266
02:30:13,520 --> 02:30:20,060
y me queda que esto se va al a0, porque este 1 + 1 = 2 se divide con un medio de a0, entonces si la f

1267
02:30:20,140 --> 02:30:27,860
es contante, el estado final del primer qubit es el estado 0 y cuando yo lo mida va a dar 0 con total

1268
02:30:27,860 --> 02:30:39,400
seguridad. Entonces, si yo nido y obtengo cero, concluyo que la F era constante.

1269
02:30:40,220 --> 02:31:07,740
Está bien? Ahora, si la F es balanceada, si la F es balanceada, esto da 1, -1 a la 1 es -1, 1 menos -1 es 1, esto se acá queda un 2, perdón, 1 menos por menos 1 es más 1, 1 más 1 es 2, se vive con 2 queda 1

1270
02:31:07,740 --> 02:31:13,160
y acá me queda -1 a la 1, que es -1, 1 -1 a 0, este termino se va.

1271
02:31:13,330 --> 02:31:16,460
Si la F es balanceada, esto es igual a 1, con lo cual si,

1272
02:31:16,560 --> 02:31:18,680
miido obtengo 1, con total seguridad.

1273
02:31:19,680 --> 02:31:23,000
Entonces, ¿en qué consiste el algoritmo cuántico?

1274
02:31:24,300 --> 02:31:27,120
Hago todo esto, todo este kilómbito y miido.

1275
02:31:27,710 --> 02:31:32,060
Si obtengo un 0, tengo certeza absoluta de que la F era constante.

1276
02:31:32,880 --> 02:31:38,100
y si obtengo uno uno tengo certeza absoluta de que la F era balanceada, ¿se entienden?

1277
02:31:38,420 --> 02:31:45,700
Bueno, ¿cuántos pasos tuve que dar un paso? El caso clásico, habíamos visto que tomaba dos pasos.

1278
02:31:49,480 --> 02:31:50,880
Me van siguiendo alguna pregunta.

1279
02:31:53,760 --> 02:31:58,620
No mate basta medirlo una vez para saber si va lanzado contante.

1280
02:31:59,110 --> 02:32:03,160
Lo malo es el nivel matemático que no entendí mucho.

1281
02:32:04,500 --> 02:32:07,320
No, bueno, pero ahora esto es común.

1282
02:32:08,710 --> 02:32:10,660
Te lo puedo decir cualquiera que estudie física,

1283
02:32:11,100 --> 02:32:15,060
general uno va a las clases y en algún momento se pierde,

1284
02:32:15,160 --> 02:32:18,340
pero la gracia es que vos o Tomás no, vos vas a tener el video esto.

1285
02:32:18,340 --> 02:32:24,200
tu vuelo puedes dar, claro, entonces vuelo que tenés que hacer después es ir y repetir estas cuentas

1286
02:32:24,500 --> 02:32:29,480
yo te voy a pasar las ya positivas, pues tenés que repetir en lápiz y papel todo lo que puedas

1287
02:32:29,700 --> 02:32:37,720
¿ok? vale, eso es lo que queda como ejercicio, pero lo que es crucial es que entiendas la idea,

1288
02:32:38,100 --> 02:32:45,700
la idea de lo que pasó, yo aplico todas estas comportas, calculo el estado del primer qubit y

1289
02:32:45,700 --> 02:32:52,840
y después miedo. Si obtengo 0 por como es la probabilidad cuántica concluyo que es

1290
02:32:53,300 --> 02:32:57,960
valencia, si contante la función y si obtengo 1 concluyo que es valenciada. En un solo paso

1291
02:32:58,280 --> 02:33:05,300
y fíjate vos que para hacer todas estas cosas yo nunca tuve que saber cuánto valía f1

1292
02:33:05,380 --> 02:33:12,740
u f de 0. Es misterioso porque yo concluyo que la f es contante valenciada sin saber

1293
02:33:12,740 --> 02:33:14,140
nada de la vez. ¿Entendés?

1294
02:33:15,680 --> 02:33:20,760
Claro, eso, yo no entiendo como un, como viste el ejemplo que voy a decir, que se repite

1295
02:33:21,220 --> 02:33:29,320
cuando te das un número y se repite, sería algo así, pero metido ya mucho más adentro.

1296
02:33:32,180 --> 02:33:37,740
Es que el nivel más, al nivel matemático, es que, que bueno, entendido capaz que no

1297
02:33:37,760 --> 02:33:41,460
podía poner palabras, pero ahora me cuesta poner palabras, lo que quiero decir.

1298
02:33:43,560 --> 02:33:49,120
Bueno, para, sigo, porque este era el caso fácil, ¿no? Ahora, ahora resolvamos el caso

1299
02:33:50,900 --> 02:33:58,400
01 al AN, ¿no? Este le va más rápido. Entonces, tenemos una F que va de 01 al AN y sabemos

1300
02:33:58,440 --> 02:34:01,760
que es constante valenciada, pero no sabemos cuál de las posibilidades ocurre. Entonces,

1301
02:34:01,920 --> 02:34:06,620
queremos determinar si es constante valenciada haciendo la menor cantidad de valaciones posibles.

1302
02:34:08,260 --> 02:34:12,160
Bien, entonces este es el ACAU y es uno de cinco para que se den la idea.

1303
02:34:13,260 --> 02:34:19,920
Entonces preparo todos los qubits en cero salvo al primer, al último que le pongo una X y lo preparo uno,

1304
02:34:20,140 --> 02:34:27,000
después aplicamos Hamar a todos, después aplicamos el oráculo, después aplicamos Hamar a los primeros,

1305
02:34:27,160 --> 02:34:29,260
salvo al último y medimos los primeros.

1306
02:34:29,720 --> 02:34:30,800
Ese es el algoritmo completo.

1307
02:34:33,420 --> 02:34:41,160
Entonces, la preparación inicial es esta, todos en 0 salgo el último que estén 1, luego le

1308
02:34:41,200 --> 02:34:50,540
aplico "hamar" a todos y esto se puede reescribir de esta manera, saco factor común el 0 menos 1,

1309
02:34:50,960 --> 02:34:58,100
esto lo pueden hacer también como ejercicio, no deberían poder hacer realmente, no es que sea muy

1310
02:34:58,100 --> 02:35:08,780
complejo, bien, ahí estamos acá, antes del oráculo, ahora aplico el oráculo, el oráculo

1311
02:35:08,800 --> 02:35:18,060
que hace al Xy me lo manda a X y suma módulo de SFX, entonces esta regla la tengo que aplicar

1312
02:35:18,180 --> 02:35:41,300
acá termino de esta suma de acá, toque aplicar, lo escribo acá, pero, toque hacer uf por si1,

1313
02:35:41,780 --> 02:35:48,420
que estoy llamando así uno arriba y esto me queda 1/10 de 2 a la n + 1 por la suma de

1314
02:35:48,480 --> 02:36:08,040
x en el 0,1 a la n por uf de x contra 0 - 1, tienen que hacer esa suma, bien. Les queda

1315
02:36:08,040 --> 02:36:14,000
esto de acá, ahí apliqué la propiedad lineal de la UF, es una transformación lineal, entonces

1316
02:36:14,410 --> 02:36:20,740
se aplica acá de término de la shimo, ahora voy a aplicar esta regla de acá, que x sirva

1317
02:36:20,800 --> 02:36:32,820
para parar a esto, ven que acá tengo UFX con el 0,1, entonces acá tienen lo que pasa

1318
02:36:32,820 --> 02:36:41,940
cada término por separado uf en un x contra 0 1 es lo mismo que x 0 f(x) menos x 1 f(1)

1319
02:36:41,940 --> 02:36:42,700
más f(x)

1320
02:36:47,220 --> 02:36:50,420
ahí están usando la

1321
02:36:56,100 --> 02:37:01,920
nada eso, esta regla de acá, esta regla de equicidio para eso y bueno

1322
02:37:07,680 --> 02:37:16,020
en el próximo paso acá de nuevo, parecido a como hacíamos antes, se acuerdan que yo en un momento los

1323
02:37:16,060 --> 02:37:25,840
convencí de estas dos líneas de acá, estas dos de acá, de forma análoga o como

1324
02:37:25,980 --> 02:37:30,020
hacíamos acá, ahora tiene que volver a hacer un rozamiento similar

1325
02:37:37,820 --> 02:37:45,260
y les va a quedar que este término de acá es lo mismo que -1 a la f(x) por x por 0 -1

1326
02:37:45,260 --> 02:37:49,640
Entonces el psi del paso 2, reemplazo eso y obtengo esto.

1327
02:37:55,180 --> 02:38:00,920
Acá lo único que hice de un paso a otro es como este 0 - 1 está en todos los

1328
02:38:01,080 --> 02:38:01,860
términos de la suma.

1329
02:38:05,960 --> 02:38:10,480
Esto es una suma, sobre todo los x y este 0 - 1 está en todos los términos, todos los

1330
02:38:10,640 --> 02:38:11,380
saco factor común.

1331
02:38:15,279 --> 02:38:15,760
bien

1332
02:38:19,460 --> 02:38:21,800
y como lo saco factor común, de vuelta

1333
02:38:22,640 --> 02:38:25,620
este 1 sobre el raíz de 2 a la n -1

1334
02:38:28,860 --> 02:38:29,880
este bichito de acá

1335
02:38:30,760 --> 02:38:32,420
un 1 sobre el raíz de 2 a la n

1336
02:38:32,540 --> 02:38:34,260
se queda acá en el primer qubit

1337
02:38:34,420 --> 02:38:36,380
y un 1 sobre el raíz de 2 se va acá

1338
02:38:37,559 --> 02:38:39,680
entonces el estado del primer qubit

1339
02:38:39,840 --> 02:38:41,340
es esto de acá

1340
02:38:43,179 --> 02:38:49,800
debido a raíz de 2 en la n, perdón no del primer qubit, de los primeros n qubits,

1341
02:38:51,080 --> 02:38:57,560
asumiendo que hay n + 1 qubits, el último qubit lo descartamos y nos quedamos con los n primeros, ¿tabian?

1342
02:39:01,140 --> 02:39:01,420
bueno

1343
02:39:06,000 --> 02:39:09,720
a este último acá al q5 si estuviera

1344
02:39:17,521 --> 02:39:23,480
en ese caso lo descarto me quedo con el estado de los primeros en equi bits

1345
02:39:24,080 --> 02:39:30,320
aplico jadamar y después mío bueno ahí le meto en el estado que venía del

1346
02:39:30,320 --> 02:39:40,500
anterior la aplico "jadamar" a todo el mundo. Cuando la aplico "jadamar" recuerden que uso

1347
02:39:40,580 --> 02:39:47,240
esta formula de acá, que x por y, ven acá, por eso yo les decía al principio que recuerden esa

1348
02:39:47,320 --> 02:39:53,761
formulita del principio que pasaba se aplicaban "jadamar" a todos los que hubies cuando cada uno

1349
02:39:53,760 --> 02:40:04,320
de los qubits no estaba en un estado que perdón, en un x que no tenga todo 0, entonces acá

1350
02:40:04,660 --> 02:40:12,400
aplique "jama", es esto de acá, acá aplico esa fórmula que les decía antes y este es

1351
02:40:12,400 --> 02:40:20,280
el estado final de los primeros n qubits, cuando mida voy a tener que calcular las probabilidades

1352
02:40:20,280 --> 02:40:33,160
con este C3 de acá, con el C3. Bien, la cuestión es que para simplificarlo, este es el estado

1353
02:40:33,240 --> 02:40:39,800
final de los primeros NQB, entonces lo que voy a hacer es medirlos y me voy a fijar si

1354
02:40:39,880 --> 02:40:46,562
obtengo la bitstring con todos ceros o no, entonces si obtengo todos ceros tengo una cosa

1355
02:40:46,560 --> 02:40:49,340
y si obtengo alguno que no sea cero tengo otra cosa.

1356
02:40:50,681 --> 02:40:58,680
Bien, acá de vuelta tengo que calcular la probabilidad de obtener todos ceros,

1357
02:40:59,460 --> 02:41:07,760
de medir o tener todos ceros. Esa probabilidad queda proporcional al coeficiente de la que tiene todos ceros

1358
02:41:07,760 --> 02:41:18,600
porque piensen que acá hay una suma, esto es una suma en donde "i" va variando, bueno, yo quiero

1359
02:41:21,480 --> 02:41:28,720
el resultado que tiene "i" igual a la bitstrain con todos 0s, bueno si es 0 esto vale 0,

1360
02:41:28,800 --> 02:41:39,480
entonces esto vale 1, me quedaste -1 a la f(x) y tengo que tener en cuenta este factor 1, 2 a la de nada.

1361
02:41:40,360 --> 02:41:45,540
Entonces la probabilidad de obtener 0 va a ser el módulo al cuadrado de ese coeficiente,

1362
02:41:46,220 --> 02:41:52,520
del coeficiente de quién, del que tiene 0, el resto no los miro. Básicamente,

1363
02:41:52,950 --> 02:41:56,399
hago una medición y me fijo que me da y estoy calculando la probabilidad de obtener todos

1364
02:41:56,400 --> 02:41:56,640
los "s"

1365
02:41:58,580 --> 02:42:01,800
ahora, ¿qué pasa acá? acá viene la parte interesante

1366
02:42:03,420 --> 02:42:04,580
si la "f" es constante

1367
02:42:12,560 --> 02:42:12,960
esto

1368
02:42:14,000 --> 02:42:16,340
o es siempre 0 o es siempre 1

1369
02:42:17,240 --> 02:42:18,220
si esto es siempre 0

1370
02:42:19,560 --> 02:42:20,900
esto suma de 1

1371
02:42:22,000 --> 02:42:24,860
2 a la n veces, entonces tengo 1 sobre 2 a la n

1372
02:42:27,180 --> 02:42:28,880
2 a la n que es 1

1373
02:42:30,400 --> 02:42:32,560
y si siempre es 1, también tengo

1374
02:42:35,119 --> 02:42:38,080
menos 2 a la n sobre 2 a la n

1375
02:42:38,680 --> 02:42:39,680
que es 1, de vuelta

1376
02:42:40,960 --> 02:42:43,140
al cuadrado, al cuadrado es 1

1377
02:42:44,040 --> 02:42:45,600
entonces si la vez es constante

1378
02:42:46,960 --> 02:42:48,300
esto de acá o es

1379
02:42:49,300 --> 02:42:57,560
0 o 1, si es 0 siempre estoy sumando 1 y si es 1 siempre estoy sumando -1, en cualquiera de los dos casos

1380
02:42:58,520 --> 02:43:04,920
tengo o 2 a la n o -2 a la n, que se cancela con el 2 a la n de abajo y obtengo 1.

1381
02:43:07,560 --> 02:43:17,440
Y atención, si la f por el contrario es balanceada, acá está sumando sobre todos los input posibles, ¿no?

1382
02:43:21,240 --> 02:43:27,160
y si la f es balanceada a veces este f(x) va a ser cero y a veces va a ser uno, la mitad

1383
02:43:27,210 --> 02:43:34,340
de las veces vale cero y la mitad de las veces vale uno, entonces cuando valga cero,

1384
02:43:37,460 --> 02:43:38,480
voy a escribir acá

1385
02:43:42,100 --> 02:43:49,600
yo tengo 1 sorreto a la n, por cuando la f valga 0 esto va a ser -1 a la 0 1

1386
02:43:51,120 --> 02:43:57,660
mas 1 mas pero cuando la f valga 1 va a valer -1, entonces algunos unos se cancelan con otros

1387
02:43:59,740 --> 02:44:04,660
ahora, ¿quiénes se cancelan con quiénes? Bueno, la mitad de las veces vale 0 y la mitad de las

1388
02:44:04,760 --> 02:44:10,700
veces vale 1, entonces hay la misma cantidad de ceros que de unos, entonces si la f es

1389
02:44:10,740 --> 02:44:16,860
balanceada, esto vale siempre 0 ¿Por qué? Porque en esta suma se alulan los 1s con los

1390
02:44:16,980 --> 02:44:23,340
-1s, porque ahí estamos usando efectivamente la condición o hipótesis de que la f era

1391
02:44:23,340 --> 02:44:36,880
la balanciada. Entonces la conclusión es que si la F es constante, entonces la probabilidad

1392
02:44:37,050 --> 02:44:47,100
de medir 0 es 1 y si la F es balanciada la probabilidad de medir 0 es 0. Entonces, corro

1393
02:44:47,140 --> 02:44:53,100
al algoritmo una vez, al algoritmo cuántico una vez, eso quiere decir que consulto al

1394
02:44:53,160 --> 02:45:01,340
oloráculo una vez sola, si obtengo todos 0 y mía, si obtengo todos 0s la función era

1395
02:45:01,420 --> 02:45:08,520
constante y si obtengo un resultado que no es todo 0 concluyo que es balanceada. En una

1396
02:45:08,580 --> 02:45:14,720
sola corrida y sin tener ni idea de cuánto vale de fe en ningún input, ¿se entienden?

1397
02:45:16,540 --> 02:45:27,180
entonces recuerden que la complejidad del algoritmo clásico era 2 a la n sobre 2 + 1, el exponencial

1398
02:45:27,220 --> 02:45:34,460
y acá la complejidad es 1, va, la complejidad de no oracular, estamos dejando de lado el

1399
02:45:34,680 --> 02:45:42,000
costo que tiene construir el oráculo, pero al menos en Query complexity, es decir, la

1400
02:45:42,000 --> 02:45:47,840
cantidad de preguntas que tengo que hacer, el clásico es exponencial y el cuántico es

1401
02:45:47,940 --> 02:45:50,440
polinomial en sentido de que tengo que hacer una pregunta sola.

1402
02:45:54,841 --> 02:46:00,420
Entonces ahí tienen en este ejemplo que no es relevante comercialmente ni sociológicamente,

1403
02:46:00,850 --> 02:46:06,500
pero sí matemáticamente, tienen un ejemplo de cómo obtendrían una ventaja utilizando

1404
02:46:06,540 --> 02:46:07,460
una computadora crítica.

1405
02:46:07,560 --> 02:46:19,640
¿Sí? Bueno, ¿por qué este algoritmo al final del día es una cagada? Bien, porque yo calculé la complejidad,

1406
02:46:20,961 --> 02:46:28,940
lo que dimos es que si querían estar completamente seguros de la solución, tenían que hacer una cantidad exponencial de evaluaciones.

1407
02:46:29,980 --> 02:46:37,300
¿Por qué? Porque tienen que evaluar la mitad más uno, como hay número exponencial de inputs listo.

1408
02:46:37,480 --> 02:46:41,500
es es potencial. Pero ¿qué pasa si permitimos una pequeña tasa de error?

1409
02:46:43,400 --> 02:46:45,600
Es decir, si resuelvo el problema

1410
02:46:50,500 --> 02:46:54,360
introduciendo la flexibilidad de que mi solución podría ser errónea.

1411
02:46:55,900 --> 02:46:59,880
Entonces vamos a ver cómo sería el algoritmo clásico, el algoritmo clásico

1412
02:47:00,790 --> 02:47:05,480
no determinista. Es decir, un algoritmo clásico que me permite

1413
02:47:05,480 --> 02:47:10,040
y se relaja un poquito y dice bueno lo voy a resolver al problema pero con una

1414
02:47:10,080 --> 02:47:12,640
probabilidad muy grande voy a dar una solución

1415
02:47:14,880 --> 02:47:19,620
que va a ser correcta con una probabilidad muy elevada, está bien? Si hago eso

1416
02:47:22,659 --> 02:47:28,980
obtengo que hay 2 a la n input posibles, hay muchos, hay potenciales y habíamos dicho

1417
02:47:29,000 --> 02:47:34,000
que la solución clásica exacta era exponencial, había que hacer 2 a la n -1

1418
02:47:34,000 --> 02:47:39,780
más uno de las redes para estar seguro. En el caso randomizado, lo que vamos a hacer

1419
02:47:39,920 --> 02:47:46,260
es fijamos un número de sed de consultas que no va a depender del tamaño del problema

1420
02:47:48,340 --> 02:47:54,240
y vamos a ir realizando evaluaciones de la función pero con inputs tomados al azar,

1421
02:47:54,440 --> 02:48:03,980
es decir, me fijo en el pool de cadenas de bits de 0 y 1 de largo n, las voy sacando

1422
02:48:03,980 --> 02:48:05,460
y luego eludó C veces.

1423
02:48:09,460 --> 02:48:10,840
Realizo C consultas.

1424
02:48:11,600 --> 02:48:12,700
Si la F era constante,

1425
02:48:13,580 --> 02:48:16,100
voy a tener que obtener que son todos 0s o todos 1s.

1426
02:48:16,160 --> 02:48:17,000
Si la F era constante.

1427
02:48:17,200 --> 02:48:18,240
Ahora si es balanceada,

1428
02:48:20,040 --> 02:48:21,020
y yo justo balanceé,

1429
02:48:21,060 --> 02:48:22,660
que yo, para fijar ideas,

1430
02:48:23,260 --> 02:48:24,440
imaginen que valoran 10 veces.

1431
02:48:24,560 --> 02:48:26,160
Ahora tienen N muy grande,

1432
02:48:26,520 --> 02:48:28,460
N igualada 50,

1433
02:48:29,020 --> 02:48:29,400
que soy yo.

1434
02:48:30,600 --> 02:48:30,860
Entonces,

1435
02:48:32,779 --> 02:48:40,200
Eligen hacer, para fijar ideas, 10 evaluaciones. Hacen 10 consultas. Si la

1436
02:48:40,300 --> 02:48:47,320
F era constante, bueno, o van a obtener 10 zeros o 10 unos. Si la F era

1437
02:48:47,400 --> 02:48:54,980
balanceada, podrían pasar dos cosas, o que justo tengan mala suerte y que las 10

1438
02:48:55,120 --> 02:48:58,980
veces que valoran, todas sean 0 o todas serán 1, o que algunas sean 0 y otras

1439
02:48:58,980 --> 02:49:03,500
serán uno de las diez veces, que yo por el que les digo, seis veces cero y cuatro

1440
02:49:03,720 --> 02:49:09,320
veces uno. Bueno, si están en ese último caso concluyen que la valenciada no hay

1441
02:49:09,340 --> 02:49:15,620
problema. Ahora, ¿qué pasaría si obtenemos todos resultados iguales pero la

1442
02:49:15,660 --> 02:49:22,841
F era valenciada? Si tenemos mala suerte, le valamos diez veces y nos da o todos

1443
02:49:22,840 --> 02:49:30,940
0 o todos 1. En ese caso, con nuestro número de evaluaciones no nos alcanza para resolver

1444
02:49:31,040 --> 02:49:37,280
el problema, pero podríamos apostar y decir, bueno, me la juego, como medio todos 0s, apuesto

1445
02:49:37,380 --> 02:49:48,601
a que Fs es val... si, perdón, que es constante. ¿Cuál es la probabilidad de que siendo balanceada

1446
02:49:48,600 --> 02:49:53,340
que ha caído en una situación así, porque esa va a ser la probabilidad del error del

1447
02:49:53,460 --> 02:50:00,240
anulismo. Si yo me la juego y digo que como obtuve 10 zeros la función era constante,

1448
02:50:00,580 --> 02:50:07,120
por eso es la balanceada, pero da una función balanceada. Si yo voy tomando inputs al azar

1449
02:50:08,420 --> 02:50:15,440
de la base de inputs, ¿cuál es la probabilidad de obtener 10 zeros en una línea? Es como

1450
02:50:15,440 --> 02:50:24,440
una moneda, una especie de moneda y otra de 10, bueno, esto está como ejercicio de

1451
02:50:24,520 --> 02:50:31,120
Nielsen-Chuang, se puede calcular. Entonces, lo problemático ocurriría, si la F es balanceada,

1452
02:50:31,380 --> 02:50:39,241
pero yo en mis evaluaciones random obtengo todos 0s o todos 1s. Y esto puede pasar ya que en general

1453
02:50:39,240 --> 02:50:45,120
se va a ser bastante más chico que 2 a la n - 1 más 1 que es la cantidad de

1454
02:50:45,200 --> 02:50:47,260
evaluaciones que necesito para resolver el problema con

1455
02:50:50,760 --> 02:50:51,800
con total certeza

1456
02:50:56,080 --> 02:51:01,020
la pregunta es si yo aún así me la juego vivo bueno la f es constante la

1457
02:51:01,040 --> 02:51:03,722
pregunta es cuál es la probabilidad de obtener una respuesta incorrecta si

1458
02:51:03,720 --> 02:51:10,600
apostamos a que es contante en ese escenario. Esto se puede calcular, entonces, dado una

1459
02:51:10,640 --> 02:51:16,920
F que sea balanceada, calculemos la probabilidad de obtener por ejemplo C inputs igual a 0.

1460
02:51:18,380 --> 02:51:23,180
Entonces, para el primero input, si lo tiro la primera vez, no, hago la primera corrida.

1461
02:51:32,860 --> 02:51:38,840
como un input al azar, evaluó la f en este input y me da 0, ¿cuál es la probabilidad

1462
02:51:38,970 --> 02:51:46,420
de que eso ocurra? La probabilidad es, como la f es balanceada, la mitad de los inputs

1463
02:51:46,640 --> 02:51:53,660
son 0 y la mitad de los outputs son 1, entonces hay 2 a la n menos 1 posibilidades de que

1464
02:51:53,780 --> 02:51:57,080
sean 0 y el total de las posibilidades es 2 a la n.

1465
02:51:58,620 --> 02:52:02,020
Entonces esta es la primera probabilidad, la probabilidad de obtener un 0.

1466
02:52:05,580 --> 02:52:10,441
Y ahora pregunto, está bien yo obtuve un 0 en la primera, cuáles lo, la probabilidad

1467
02:52:10,440 --> 02:52:18,180
de volver a obtener un 0. Ahora tengo de todos los 0 posibles que eran n-1, ya saqué 1, ya lo obtuve.

1468
02:52:19,020 --> 02:52:27,380
Entonces me quedan 2^n-1 menos 1, 0 es posible. Y cuántas posibilidades tengo, 2^n-1, porque ya la estiré.

1469
02:52:28,260 --> 02:52:36,560
Y bueno, y así siguiendo, la probabilidad de obtener el tercer 0 va a ser 2^n-1 menos 2, dividido 2^n-2.

1470
02:52:38,680 --> 02:52:48,720
Y en general la probabilidad de obtener el 0/c/10 va a ser esta fórmula de acá, esto les queda como ejercicio convencerse.

1471
02:52:49,920 --> 02:52:57,380
Y entonces si la función es balanceada, la probabilidad de obtener c0's consecutivos es el producto de todas estas probabilidades.

1472
02:52:57,940 --> 02:53:01,660
¿Qué se puede escribir de forma compacta con la productoria?

1473
02:53:01,760 --> 02:53:04,240
ya lo habíamos discutido en otra clase a esto

1474
02:53:07,420 --> 02:53:11,360
y la realidad es que entonces cuando eres muy grande cada uno de estos términos

1475
02:53:11,500 --> 02:53:16,980
fíjense lo hago para este de acá esto es lo que se acuerdan cuando calculaban

1476
02:53:17,080 --> 02:53:19,260
límites en algún momento de su vida

1477
02:53:22,640 --> 02:53:27,682
hacía algo parecido a esto esto es lo mismo que dos ala en

1478
02:53:29,000 --> 02:53:35,960
no, perdón, saco factor como el 2aln, esto me queda 1/2 menos c-1 sobre 2aln

1479
02:53:38,121 --> 02:53:44,480
dividido 2aln por 1 menos c-1 sobre 2aln

1480
02:53:45,340 --> 02:53:50,900
entonces esto tiende a cero cuando eres muy grande, tiende a cero, este se va con este

1481
02:53:51,600 --> 02:53:57,441
entonces esto cuando eres muy grande se parece un medio, ese es el punto

1482
02:53:57,800 --> 02:54:02,260
Entonces ustedes tienen que hacer el producto básicamente de un medio por un medio por un medio por un medio

1483
02:54:06,340 --> 02:54:10,080
y esto les queda uno sobre dos a la c, entonces recapitulando

1484
02:54:12,240 --> 02:54:20,960
si la funciona balanceada y hacemos c evaluaciones al azar y obteníamos obteníamos c0 la probabilidad

1485
02:54:21,000 --> 02:54:32,800
de que ocurre ese evento es 1/2C, si por ejemplo si C = 10, bueno, que hacen 10 evaluaciones,

1486
02:54:33,320 --> 02:54:45,620
entonces 1/2C es 1/2C es 1/10, es 1/1024 y si en general este número tiende a 0 muy

1487
02:54:45,640 --> 02:54:53,600
rápido cuando aumentan el C. Entonces la probabilidad de error es abrumadoramente baja.

1488
02:54:55,700 --> 02:55:05,180
El problema del algoritmo de este de Doi Chosa es que la complejidad del algoritmo es C y es

1489
02:55:05,260 --> 02:55:12,842
constante, no depende del tamaño del problema. Entonces, dado que existe esta solución clásica

1490
02:55:12,840 --> 02:55:17,860
que permite un poquito de error, pero con una prueba de idea muy baja, esto hace que el algoritmo

1491
02:55:18,180 --> 02:55:24,300
cuántico sea inútil, porque existe este algoritmo clásico que es muy barato y es eficiente,

1492
02:55:24,760 --> 02:55:31,660
resuelve el problema de forma eficiente, si permitimos una pequeñata error. Bueno, como ven,

1493
02:55:33,580 --> 02:55:41,322
ya hemos llegado al límite temporal, nos hemos pasado, y como ven, ya las cuentas se vuelven un

1494
02:55:41,320 --> 02:55:49,120
un poquito más complicada, pero acá es crucial que lean este mismo ejemplo de Nielsen Chuang

1495
02:55:49,650 --> 02:55:58,480
y que vean de vuelta mi clase, ¿sí? Y traten de entenderlo más posible. Pero esta es la

1496
02:55:58,520 --> 02:56:04,240
idea de los algoritmos cuánticos y este ejemplo debería darles una idea de por qué uno puede

1497
02:56:04,380 --> 02:56:05,940
sacar ventaja con computadoras cuánticos.

1498
02:56:08,820 --> 02:56:14,840
¿Y eso de uno, pues mejorar tu computadora cuántica para que sea más eficiente después

1499
02:56:15,440 --> 02:56:17,160
o es improbable?

1500
02:56:18,340 --> 02:56:18,740
¿Cómo, cómo?

1501
02:56:19,440 --> 02:56:24,340
Que viste que ahí pudiste probar, bueno, mostrarte que plásticamente lo podía ser

1502
02:56:24,680 --> 02:56:29,860
muy eficiente, ya no te conviene una computadora cuántica, pero puede ser que el encepturo

1503
02:56:30,700 --> 02:56:32,780
se convenga o muy improbable.

1504
02:56:32,880 --> 02:56:39,920
No, claro, este es un ejemplo sencillo de juguete, solo para mostrarte a vos que podría haber una

1505
02:56:39,960 --> 02:56:45,740
ventaja en la computadora. Pero después hay otros algoritmos que sí son útiles, ¿entendés?

1506
02:56:46,160 --> 02:56:46,380
¿Cuántos?

1507
02:56:47,040 --> 02:56:48,800
Ah, eso se necesita mucho más.

1508
02:56:48,800 --> 02:56:53,920
Este es. Claro, pero lo vamos a ver, no te preocupes, lo vamos a tratar de explicar de

1509
02:56:53,920 --> 02:56:55,900
la forma lo más sencilla posible, ¿ok?

1510
02:56:58,240 --> 02:57:03,340
pero vos primero, quédate con esto, quédate con que viste un ejemplo de

1511
02:57:03,440 --> 02:57:07,780
el límite cuántico para un problema ficticio que haga lo suficientemente sencillo como

1512
02:57:07,840 --> 02:57:12,180
para que hagamos todas las cuentas, ya a los otros va a ser más difícil hacer todas las cuentas,

1513
02:57:12,400 --> 02:57:12,580
¿entendés?

1514
02:57:13,260 --> 02:57:13,380
Sí.

1515
02:57:15,060 --> 02:57:16,480
Pero la idea la vas a entender.

1516
02:57:18,300 --> 02:57:22,620
Bueno, en este no, la cuenta no es que sean difíciles, sino que, ya muy rápido.

1517
02:57:22,760 --> 02:57:23,140
Son muchas.

1518
02:57:23,920 --> 02:57:24,520
Sí, eran muchas.

1519
02:57:24,920 --> 02:57:28,140
pero que agravado, puedo ver de vuelta.

1520
02:57:30,721 --> 02:57:32,340
La vez en cámara lenta.

1521
02:57:33,580 --> 02:57:36,240
Sí, sí, mañana subo las de Apositio.

1522
02:57:40,000 --> 02:57:43,080
Y subo el vídeo, acá Sebastián siempre

1523
02:57:43,961 --> 02:57:46,700
ayudando, grababa las clases, un genio,

1524
02:57:47,330 --> 02:57:49,720
así que bueno, él me la pasa mañana y yo subo el vídeo.

1525
02:57:51,681 --> 02:58:04,040
Así que bueno gente eso, eso es todo por hoy, no le aflojen, hicieran leccion del libro, mañana le subo todo video y apositivas de las clases.


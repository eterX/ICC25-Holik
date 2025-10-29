
```srt
1
00:00:00,001 --> 00:00:00,900
¿Hay que instalar el flat pack?

2
00:00:02,979 --> 00:00:04,480
-Flat pack, así se llama.

3
00:00:05,540 --> 00:00:08,340
-Sí, hay que instalar el flat pack, que es el manejador de paquetes,

4
00:00:09,000 --> 00:00:12,360
digamos así, Copy&Ride, tipo contener y sal.

5
00:00:12,919 --> 00:00:14,540
-Ahora sí, tenés que tener la aplicación.

6
00:00:17,080 --> 00:00:18,060
-¿Dónde? -Uno más, para arriba.

7
00:00:19,720 --> 00:00:21,680
-Uno más, para arriba. -Oca, esto.

8
00:00:24,019 --> 00:00:27,500
-No, no, no, el comandito de instalación.

9
00:00:28,000 --> 00:00:31,540
el otro el que tenías en el navegador, en el gel

10
00:00:32,300 --> 00:00:32,520
este

11
00:00:33,940 --> 00:00:34,320
ah

12
00:00:35,820 --> 00:00:37,200
ah que tonto, ahí

13
00:00:38,340 --> 00:00:38,900
cual, este

14
00:00:40,260 --> 00:00:40,320
no

15
00:00:41,500 --> 00:00:41,740
este

16
00:00:42,400 --> 00:00:46,320
a ver, ese, el de install, el flat pack install

17
00:00:46,880 --> 00:00:47,700
creo que ese no

18
00:00:48,300 --> 00:00:50,180
no, ese es el ppa, ahí, ese

19
00:00:50,680 --> 00:00:51,940
flat pack install

20
00:00:57,500 --> 00:00:57,980
no

21
00:00:57,980 --> 00:01:01,820
y iba a grabar, alguien se conectó y iba a grabar.

22
00:01:09,119 --> 00:01:11,980
Ya diría que no grabaremos total.

23
00:01:13,320 --> 00:01:16,240
Acá en Procap, Raúl y Martínez están grabando.

24
00:01:17,140 --> 00:01:18,300
Perfecto, bueno listo.

25
00:01:19,640 --> 00:01:24,820
Bueno, entonces hoy vamos a ver el formalismo cuántico,

26
00:01:24,980 --> 00:01:26,880
pero muy lento, muy, muy lento.

27
00:01:27,680 --> 00:01:31,340
Perdón para gente como Alejandro que ya había visto esto en otros lados,

28
00:01:31,960 --> 00:01:38,600
pero lo vamos a dar muy despacio, porque como en este curso va a haber examen,

29
00:01:39,940 --> 00:01:42,000
es muy importante que entiendan el geolineal.

30
00:01:42,380 --> 00:01:47,220
Entonces, vamos a detenernos bastante en la parte matemática de todo esto.

31
00:01:49,980 --> 00:01:54,960
Entiendo que es aburrido, muchas veces, a veces la matemática puede llegar a ser

32
00:01:54,960 --> 00:02:01,380
pero vale la pena hacer el esfuerzo porque estas cuentas que van a aprender

33
00:02:03,420 --> 00:02:08,380
muy probablemente les sirvan para otras materias de la carrera y también les

34
00:02:08,479 --> 00:02:12,380
puedes abrir el trabajo para muchos de para quienes se vayan a dedicar a la

35
00:02:12,420 --> 00:02:18,060
programación saber al general lineal entender matrices poder entender cosas

36
00:02:18,180 --> 00:02:22,040
básicas de espacios vectoriales siempre es una gran herramienta entonces no lo

37
00:02:22,040 --> 00:02:26,660
tomen como de obrido sino como adquirir una nueva capacidad.

38
00:02:27,840 --> 00:02:28,240
Así que bueno.

39
00:02:29,550 --> 00:02:33,840
Bien, vamos a empezar primero para motivar viendo el ejemplo de

40
00:02:33,840 --> 00:02:40,400
la doble rendija, que es un ejemplo que intenta reflejar

41
00:02:41,620 --> 00:02:44,940
algunas características básicas de los sistemas cuánticos.

42
00:02:46,060 --> 00:02:49,840
Entonces, imaginen que tienen una fuente que está ilustrada

43
00:02:49,840 --> 00:02:55,100
como una especie de corneta que va a tirar primero pelotas, pelotas como se

44
00:02:55,140 --> 00:03:01,180
fueran bolitas de las que se usaban para jugar cuando eran chicos, pelotitas

45
00:03:01,540 --> 00:03:06,760
o pequeños bolitas de público, que se lloró que sea y estas pelotas se van a ir

46
00:03:06,780 --> 00:03:10,720
tirando de alguna para ir para adelante con alguna dispersión

47
00:03:13,180 --> 00:03:17,560
y van a pasar por dos rendijas, la rendija de la izquierda y la rendija de la

48
00:03:17,560 --> 00:03:22,380
derecha, si es donde está azul no pueden pasar las pelotas, solo pueden pasar por las rendijas.

49
00:03:23,070 --> 00:03:29,760
Y nosotros vamos a ir en este experimento ideal detectando dónde impacta cada una de las pelotas

50
00:03:30,430 --> 00:03:37,520
en una pantalla que hay atrás de todo. Primero lo vamos a describir lo que ocurre con pelotas

51
00:03:37,600 --> 00:03:42,920
clásicas, con pelotas macroscópicas que ustedes podrían agarrar con la mano y después qué

52
00:03:42,920 --> 00:03:46,380
que pasaría si repetiríamos el experimento con sistemas cuánticos.

53
00:03:47,060 --> 00:03:50,160
Entonces ahí están las pelotas que salen, ven que algunas pasan por la

54
00:03:50,280 --> 00:03:55,280
red de izquierda, otras por la derecha. Estas como son pelotas clásicas pueden

55
00:03:55,520 --> 00:03:58,740
ver por dónde va cada una, tienen trayectorias bien definidas.

56
00:04:00,650 --> 00:04:04,980
En el caso cuántico no vamos a poder ver las trayectores de las pelotas, sino

57
00:04:05,380 --> 00:04:08,700
vamos a ver solo cuando impactan en la segunda pantalla.

58
00:04:10,180 --> 00:04:12,400
Entonces ven, algunas van por la izquierda, otras por la derecha.

59
00:04:13,120 --> 00:04:16,620
Consecuentemente, algunas van a caer, cuando las detectamos en la segunda pantalla,

60
00:04:17,660 --> 00:04:22,100
algunas van a ir cayendo a la izquierda y otras van a la derecha.

61
00:04:23,020 --> 00:04:29,680
Ahora bien, ¿qué pasaría si en vez de tirar pelotitas bolitas o pelotas de pul,

62
00:04:30,660 --> 00:04:34,060
tiráramos efectivamente y si damos el mismo experimento con sistemas cuánticos?

63
00:04:34,860 --> 00:04:38,540
Este experimento se puede hacer, tiene un equivalente con electrones,

64
00:04:38,640 --> 00:04:43,560
también tiene un equivalente con fotones, se puede hacer también con neutrones, se

65
00:04:43,640 --> 00:04:51,140
conoce como el experimento del adole rendijo. Entonces, si vamos tirando a las partículas

66
00:04:51,140 --> 00:04:58,040
de 1, ahora partículas cuánticas, vamos a ir detectando que estas caen, vamos a, en

67
00:04:58,040 --> 00:05:07,679
la segunda pantalla, vamos a ir viendo eventos de detección de 1 y en vez de tener

68
00:05:08,660 --> 00:05:13,980
dos franjas, tengo varias y esta física se conoce como un patrón de interferencia,

69
00:05:14,770 --> 00:05:23,840
es como si esta rendija hubiese actuado de, es como si las partículas se comportaran de

70
00:05:23,860 --> 00:05:29,900
forma ondulatoria, como si fuera luz y al final tuviéramos un patrón de interferencia,

71
00:05:30,250 --> 00:05:35,959
que no es esperable porque las partículas van siendo detectadas de una, de repente

72
00:05:35,960 --> 00:05:38,820
tengo un...hace una pantalla, en el centro de alguien.

73
00:05:43,380 --> 00:05:44,960
Esto ya le voy cerrando.

74
00:05:55,420 --> 00:06:01,300
A los sistémitas cuánticos les voy detectando la 1 y van cayendo y una

75
00:06:01,360 --> 00:06:05,940
esperaría que en realidad tengamos 2 franjas, una la que corresponde a las que

76
00:06:05,940 --> 00:06:11,040
pasaron por la, por la rendija izquierda y la otra franja que corresponderá es que

77
00:06:11,080 --> 00:06:15,780
pasan por la rendija derecha, pero no, lo que vemos es un patrón más complejo, sí.

78
00:06:17,360 --> 00:06:21,660
Entonces las partículas van cayendo más o menos en unas franjitas que se

79
00:06:21,700 --> 00:06:27,200
conocen como franjas de interferencia, sí. Y fíjense una cosa, si me concentro

80
00:06:27,220 --> 00:06:32,260
por ejemplo en el pico del medio, en esta franja del medio, una partícula que

81
00:06:32,260 --> 00:06:37,420
que cayó acá, yo no puedo dirimir, por ejemplo, esta si vino de la rendija

82
00:06:37,480 --> 00:06:43,620
izquierda o de la rendija derecha, en general el patrón de interferencia me

83
00:06:43,700 --> 00:06:49,680
impide decidir a partir de lo que observo en la pantalla de atrás por qué

84
00:06:49,700 --> 00:06:56,740
rendija pasó la partícula en la primera pantalla. Entonces ustedes dirán

85
00:06:56,740 --> 00:07:02,820
Bueno, para responder esa pregunta, es decir, para ver por qué rendija pasó cada partícula,

86
00:07:03,120 --> 00:07:11,480
coloquemos unos aparatos de medición. Uno en una rendija, el otro en la otra, estos anillos serían,

87
00:07:11,850 --> 00:07:19,000
por ejemplo, un anillo por el cual circulan al corriente cuando pasa una partícula cargada,

88
00:07:19,330 --> 00:07:24,180
el mecanismo físico ahora no nos interesa. Lo que es importante es que estos anillos indican

89
00:07:24,180 --> 00:07:30,080
que ahora puse un aparato de medición para dirimir por qué rendija pasó cada

90
00:07:30,160 --> 00:07:36,420
partícula. Bueno, cuántica, estamos en el régimen cuántico, entonces voy a tirar de

91
00:07:36,420 --> 00:07:40,480
a uno, voy a hacer el experimento tirando a los sistemitas cuánticos de a uno de nuevo

92
00:07:41,180 --> 00:07:47,580
y me voy a ir fijando qué detecto en la segunda pantalla. Ahora puse aparatos de medición en

93
00:07:47,580 --> 00:07:54,880
la primera pantalla, bueno, voy tirando, detecto una, detecto otra, detecto una, es decir, los

94
00:07:55,000 --> 00:08:01,440
eventos de detección son aleatorios, sin embargo debido al hecho de que puse los aparatos de

95
00:08:01,460 --> 00:08:09,460
medición para debilidad, ¿por qué rendija pasó cada partícula? Ahora en cada tirada yo sé que tal

96
00:08:09,540 --> 00:08:14,939
partícula fue por la izquierda o que tal partícula fue por la derecha, pues entonces ahora ya no

97
00:08:14,940 --> 00:08:20,780
observo más el patrón de interferencia. Lo que observo es lo que hubiese observado

98
00:08:21,050 --> 00:08:27,160
si el sistema fuera clásico. Es decir, si tiramos bolitas clásicas veríamos algo muy

99
00:08:27,220 --> 00:08:31,800
parecido a esto ¿no? Porque algunas bolitas serían por la izquierda, otras por la derecha

100
00:08:31,800 --> 00:08:39,620
y veríamos las dos sombras de las dos rendijas. Sin embargo, en el caso cuántico, cuando no

101
00:08:39,680 --> 00:08:44,099
pongo nada veo un patrón de interferencia y cuando pongo los aparatos de medición

102
00:08:44,099 --> 00:08:54,100
se destruye el patón de interferencia y veo otra distribución de pelotitas.

103
00:08:55,620 --> 00:08:57,080
Ven acá puse para comparar.

104
00:08:57,860 --> 00:09:01,400
Si no pongo los aparatos de medición, observó patón de interferencia.

105
00:09:01,600 --> 00:09:07,100
Si pongo aparatos de medición, se destruye el patón de interferencia

106
00:09:07,180 --> 00:09:09,360
y obtenga un comportamiento de tipo partícula,

107
00:09:09,420 --> 00:09:12,660
porque ahí puedo decir que algunas fueron por la izquierda y otras por la derecha.

108
00:09:12,900 --> 00:09:18,680
por ejemplo, las que golpearon acá, digo que venían de la izquierda y las que detecto acá, digo que venían por la derecha.

109
00:09:19,600 --> 00:09:29,560
Bien, entonces, algunas consideraciones acerca de lo que estuvimos discutiendo de este experimento.

110
00:09:30,920 --> 00:09:39,280
Distintos contactos de experimentación son incompatibles entre sí, porque o pongo aparatos de menición o no los pongo.

111
00:09:40,700 --> 00:09:47,440
Si un experimento corresponde a ir haciendo pasar las partículas de una, sin poner los

112
00:09:47,560 --> 00:09:52,240
aparatos que detectan por qué el del mijaco pasó y otro experimento incompatible con

113
00:09:52,240 --> 00:09:54,880
el primero es poner el aparato de la ericción.

114
00:09:56,920 --> 00:10:02,360
La otra cosa importante es que en ambos casos, en ambos contextos de experimentación, el

115
00:10:02,380 --> 00:10:09,880
comportamiento es probabilístico porque cuando ve tirando las pelotitas, si hago el experimento

116
00:10:09,880 --> 00:10:16,080
yo no puedo predecir o al menos la mecánica cuántica no me permite predecir a dónde va a

117
00:10:16,200 --> 00:10:19,580
ser detectada la segunda pantalla de la partícula, yo tiro una y bueno,

118
00:10:19,640 --> 00:10:24,180
estoy detectada y tiro otra y es detectada ya y así hay una dispersión

119
00:10:28,760 --> 00:10:34,540
o hay una distribución de probabilidad que gobierna el comportamiento de las partículas y

120
00:10:34,540 --> 00:10:40,700
la cuántica, adelanto, me permite calcular esa distribución de probabilidad.

121
00:10:41,920 --> 00:10:47,080
Entonces, ya sea en este caso, como en el otro, cuando no pongo los aparatos, ahí también

122
00:10:47,260 --> 00:10:52,180
tengo un comportamiento probabilístico. Es decir, van cayendo de forma aleatoria, no

123
00:10:52,180 --> 00:10:58,380
lo puedo predecir. Y se me arrube un patrón. Cíjense que a esto lo pueden pensar como una,

124
00:10:59,180 --> 00:11:04,040
digamos, a la densidad de bolitas detectadas en la segunda pantalla la

125
00:11:04,180 --> 00:11:06,040
pueden pensar como una densidad de probabilidad.

126
00:11:06,220 --> 00:11:09,580
Hoy vamos a discutir probabilidad al final, así que no se preocupen demasiado.

127
00:11:10,640 --> 00:11:11,480
Vamos a hablar del tema.

128
00:11:13,680 --> 00:11:19,140
Porque imagino que muchos y muchas de ustedes no saben nada de teoría de

129
00:11:19,140 --> 00:11:23,460
probabilidades, pero bueno, más o menos piensen que cuando tiran un lado,

130
00:11:23,720 --> 00:11:28,100
el lado tiene comportamiento probabilístico, porque cuando lo tiran

131
00:11:28,100 --> 00:11:33,060
puede salir cualquiera de las caras del 1 en 6 y cada una sale con una cierta probabilidad.

132
00:11:33,060 --> 00:11:35,760
Y ustedes no pueden predecir que cara va a salir.

133
00:11:36,040 --> 00:11:39,260
Si pueden predecir en base a estudiar el lado,

134
00:11:40,250 --> 00:11:42,980
la probabilidad con la cual puede salir cada cara.

135
00:11:43,120 --> 00:11:46,520
Típicamente si el lado es justo, si está bien armado,

136
00:11:47,400 --> 00:11:49,460
cada cara sale con probabilidad un sexto.

137
00:11:50,390 --> 00:11:51,220
Y acá pasa lo mismo.

138
00:11:53,100 --> 00:11:57,800
cada partícula va a ser detectada en la segunda pantalla con una cierta probabilidad

139
00:11:59,860 --> 00:12:02,400
y esa probabilidad se puede calcular usando la cuántica

140
00:12:02,900 --> 00:12:07,600
pero la cuántica en una tirada individual no me dice dónde va a caer cada partícula

141
00:12:07,860 --> 00:12:09,260
no me dice dónde va a ser detectada

142
00:12:09,920 --> 00:12:15,380
es decir, no se pronuncia acerca de lo que ocurre en eventos individuales

143
00:12:17,840 --> 00:12:26,560
Entonces, este comportamiento probabilístico sí es descrpto por la cuántica.

144
00:12:27,460 --> 00:12:32,960
La cuántica permite calcular las distribuciones de probabilidad asociadas a cada uno de los dos experimentos.

145
00:12:33,140 --> 00:12:38,700
Entonces, hay distintos contextos de experimentación que son incompatibles entre sí.

146
00:12:40,500 --> 00:12:44,620
Hay un comportamiento probabilístico en ambos contextos.

147
00:12:46,000 --> 00:12:51,140
Y la cuántica me permite describir las distribuciones de probabilidad en cada contexto de experimentación.

148
00:12:52,200 --> 00:12:55,780
Y la otra cosa relevante que les tiene que quedar bien grabada es que

149
00:12:56,520 --> 00:13:01,560
las distribuciones de probabilidad dependen del contexto de experimentación.

150
00:13:03,120 --> 00:13:08,000
Si cambio el experimento, voy a tener otras probabilidades para los eventos.

151
00:13:09,700 --> 00:13:15,160
Ahora, la otra cosa interesante es que si decido hacer un experimento de forma tal de

152
00:13:15,160 --> 00:13:19,760
medir por qué rendija pasó la partícula, se destruye el patón de interferencia.

153
00:13:20,460 --> 00:13:24,040
Y si no lo hago, voy a observar un patón de interferencia,

154
00:13:24,480 --> 00:13:28,040
pero pierdo información acerca del camino que tomó la partícula,

155
00:13:28,080 --> 00:13:31,080
porque no sé si fue por la rendija izquierda o la rendija derecha.

156
00:13:32,680 --> 00:13:33,080
Entonces, bueno,

157
00:13:36,460 --> 00:13:40,240
cuando se descubrió la mecánica cuántica, se hicieron un montón de...

158
00:13:40,600 --> 00:13:44,019
Se empezó a acumular un montón de evidencia empírica

159
00:13:45,040 --> 00:13:47,920
en favor de este comportamiento probabilístico.

160
00:13:48,500 --> 00:13:48,640
¿Verdad?

161
00:13:53,100 --> 00:13:54,640
¿Cómo vamos por acá por el mit?

162
00:13:54,880 --> 00:13:54,980
¿Bien?

163
00:13:56,890 --> 00:13:57,580
¿Hagamos una pregunta?

164
00:13:58,420 --> 00:13:59,240
Bien, vamos a ver ahora.

165
00:14:00,600 --> 00:14:01,360
Bien, perfecto.

166
00:14:02,960 --> 00:14:04,840
No se queden con preguntas, ¿eh?

167
00:14:04,890 --> 00:14:07,900
De nuevo, este curso tiene parciales.

168
00:14:08,720 --> 00:14:10,860
Significa, al aprobar el curso,

169
00:14:11,030 --> 00:14:12,220
hay que aprobar los parciales.

170
00:14:13,020 --> 00:14:17,880
no vienen a las clases y se sacan unése los parciales. No me importa. Por ahí vienen a las

171
00:14:18,080 --> 00:14:23,140
clases y se sacan un solo en los parciales. Por sí me importa, pues quiero que aprueben, pero lo que

172
00:14:23,180 --> 00:14:29,120
quiero decir es que usen las clases para hacer preguntas, ok? La idea es que interactivamente,

173
00:14:29,580 --> 00:14:33,420
todos los martes, ustedes me vayan preguntando cosas a mí y por supuesto me pueden mandar también

174
00:14:33,480 --> 00:14:38,960
por el chat y por WhatsApp o por donde sea. Me pueden mandar preguntas o seguir discutiendo,

175
00:14:39,020 --> 00:14:45,300
pero es importante que ustedes tomen en las manos la tarea de aprender, no es solo mirar las clases

176
00:14:45,420 --> 00:14:51,260
porque así no van a probar los parciales, es importante que ejerciten, que hagan ejercicio,

177
00:14:51,720 --> 00:14:59,680
hoy vamos a hacer bastante ese ejercicio. Bien, sigo, lo que se descubrió al final, a partir de

178
00:15:00,020 --> 00:15:06,899
estudiar muchos experimentos y de pensar y pensar, es que primero que el comportamiento tenía que

179
00:15:10,080 --> 00:15:14,580
que se tiene que construir no quedaba otra más que hacerla probabilística.

180
00:15:15,040 --> 00:15:19,900
Y la otra cosa, que por ahí es un tanto precubular de la física cuántica,

181
00:15:19,980 --> 00:15:25,320
es que para describir estas probabilidades se utilizaron espacios de Hilbert,

182
00:15:26,200 --> 00:15:32,000
es una herramienta matemática que está vinculada a los espaccios vectoriales.

183
00:15:32,120 --> 00:15:35,240
Y es lo que voy a explicar hoy. Hoy voy a hablar de espacios vectoriales.

184
00:15:36,820 --> 00:15:42,780
y vectores y matrices y cómo se suman y todo eso, así que tengan paciencia porque vamos a hacer

185
00:15:42,960 --> 00:15:49,640
cuentas. ¿Por qué? Bueno, porque en la física en general uno va a querer dar una descripción

186
00:15:50,200 --> 00:15:58,680
matemática de los fenómenos, por ejemplo, vamos al lapizarro. Piensen como es la física clásica,

187
00:15:58,720 --> 00:16:07,020
¿no? Ustedes tienen una pelotita, en un momento inicial la pelotita va a estar en el espacio,

188
00:16:07,100 --> 00:16:13,540
que es eso, entonces ustedes que hacen ponen un sistema de coordenadas x y z y dan las coordenadas

189
00:16:13,540 --> 00:16:24,519
de la pelotita, ¿no? Entonces dicen que es eso, a un tiempo t, a un tiempo inicial, la

190
00:16:24,520 --> 00:16:37,700
la pelotita está a una altura de tanto en z, que es yo, vamos a poner z0 de altura y en la dirección

191
00:16:37,800 --> 00:16:46,700
x está en x0 y en la dirección y están y0, esto sería si ustedes están acá y le quieren

192
00:16:46,880 --> 00:16:53,920
decir a una persona que vaya a la pelotita le dicen bueno caminen tantos metros en x, después caminen

193
00:16:53,920 --> 00:16:57,980
tanto metros en "y" y caminen tanto metros en "z", y van a llegar a la pelotita.

194
00:16:59,580 --> 00:17:03,480
Ahora la pelota va a estar sujeta a fuerzas y se va a estar moviendo.

195
00:17:03,640 --> 00:17:13,480
Entonces la posición inicial, llamamos la "x" o llamamos la "x", va a ser un vector

196
00:17:13,800 --> 00:17:19,880
con tres componentes, "x0" y "0" y "z0". Eso es a un tiempo inicial, pero la pelota

197
00:17:19,880 --> 00:17:28,079
se va a mover en el tiempo. ¿Por qué? Bueno, porque va a tener una velocidad. A cada instante

198
00:17:28,079 --> 00:17:35,560
del tiempo va a haber una velocidad. La velocidad se define como la derivada de la posición

199
00:17:35,780 --> 00:17:41,120
respecto del tiempo. Es también otro vector. Entonces, para dar el estado de movimiento

200
00:17:41,290 --> 00:17:46,960
de la partícula, nos tiene que dar, por ejemplo, la posición y la velocidad. Esto es el estado.

201
00:17:51,080 --> 00:17:58,500
entonces ustedes en la física clásica van a estar interesados en dar, calcular cuál va a ser la

202
00:17:58,540 --> 00:18:07,040
trayectoria de una pelota o un planeta o un cuerpo en general en función de las fuerzas que actúan

203
00:18:07,040 --> 00:18:17,040
sobre ese cuerpo. Y para, por ejemplo, ustedes conocerán las leyes del Newton, M por aceleración,

204
00:18:17,360 --> 00:18:23,240
masa por aceleración es igual a la sumatoria de la fuerza sobre un cuerpo. Y a partir de

205
00:18:23,320 --> 00:18:28,520
esta ecuación, ustedes pueden calcular la trayectoria de un cuerpo. Y esta ecuación

206
00:18:28,520 --> 00:18:33,800
es del terminista, si ustedes conocen las condiciones iniciales, pueden predecir todo

207
00:18:33,800 --> 00:18:44,780
momento a futuro, etcétera, etcétera. Pregunta, ¿Hay alguien para quien esto sea rarísimo y no lo

208
00:18:44,920 --> 00:18:51,520
hayan visto nunca? No tengan vergüenza en contestar, no los estoy evaluando, simplemente es para tener

209
00:18:51,640 --> 00:19:00,520
una idea de cómo son los alumnos. Igual en este curso no vamos a ver física, clásica, pero cuento

210
00:19:00,520 --> 00:19:08,140
esto para que se entienda qué hacemos los físicos, en física lo que se hace es dar una descripción

211
00:19:08,540 --> 00:19:13,300
de los fenómeros, por ejemplo cómo se muer un planeta, por ejemplo cómo se muer una bola de

212
00:19:13,320 --> 00:19:18,640
pul o cómo se muer un auto. Para hacer eso damos una descripción matemática, medimos cosas,

213
00:19:19,540 --> 00:19:25,860
posiciones, velocidad, temperaturas, energía, lo que se mide en cosas. A partir de lo que se mide,

214
00:19:26,980 --> 00:19:32,280
como se conocen, cuáles son las fuerzas que actúan sobre los cuerpos, se hacen cálculos y se

215
00:19:32,320 --> 00:19:38,860
calculan trayectorias y con eso se puede predecir lo que va a pasar, perfecto, claro,

216
00:19:39,120 --> 00:19:45,820
mañana dice haberlo visto es una cosa acordarse de otra, bueno, claro, totalmente, es totalmente así,

217
00:19:46,300 --> 00:19:51,180
lo importante es que en física damos una descripción matemática de los fenómenos,

218
00:19:54,220 --> 00:19:59,740
Entonces por ejemplo en física clásica usamos un vector de tres componentes para dar la posición

219
00:19:59,790 --> 00:20:07,560
de un cuerpo en el espacio, esto deberían poder entenderlo, si yo planto tres direcciones que

220
00:20:07,600 --> 00:20:15,280
llamo x y y z, perpendiculares entre sí, con estas tres direcciones yo puedo ubicar cualquier cosa

221
00:20:15,460 --> 00:20:21,200
porque digo caminad tantos metros o centímetros en x, tantos metros o centímetros en y, tantos

222
00:20:21,200 --> 00:20:27,000
metos en Z, con esos tres números yo puedo dar la ubicación de cualquier otro cuerpo.

223
00:20:28,550 --> 00:20:36,600
Y bueno, sobre los cuerpos típicamente actúan fuerzas y si uno conoce esas fuerzas utilizando

224
00:20:36,600 --> 00:20:44,720
las leyes de Newton que tienen esta pinta uno puede calcular el movimiento futuro de los cuerpos.

225
00:20:44,760 --> 00:20:48,040
Entonces lo que hace es dar una descripción matemática.

226
00:20:48,880 --> 00:20:54,460
¿Qué pasa en cuántica? Bueno, en cuántica les decía no tenemos el concepto de trayectoria.

227
00:20:56,340 --> 00:21:02,640
No está el concepto de trayectoria porque nunca podemos medir la velocidad y la posición al mismo tiempo.

228
00:21:04,440 --> 00:21:10,880
Y base en general, lo que termina pasando es que nunca podemos medir en cuántica variables

229
00:21:10,880 --> 00:21:17,520
con jugadas al mismo tiempo. Entonces, sea como sea el sistema que estamos describiendo, no va a haber

230
00:21:17,600 --> 00:21:24,220
una trayectoria a describir. Pero en cuántica estamos citados en calcular probabilidades,

231
00:21:25,100 --> 00:21:32,300
probabilidades de ocurrencia de eventos. Entonces la descripción cambia completamente porque en

232
00:21:32,300 --> 00:21:38,040
vez de decir "dame las fuerzas, dame las condiciones iniciales y yo te voy a predecir el movimiento

233
00:21:38,040 --> 00:21:45,140
la futura lo que decimos es, dame las características del sistema, dame su estado inicial, y a partir

234
00:21:45,140 --> 00:21:50,140
de eso y las fuerzas actuales yo te voy a calcular la probabilidad de que ocurra tal

235
00:21:50,140 --> 00:21:56,780
o cual cosa, es una descripción probabilística. Para hacer una analogía, si tuvieran un dado

236
00:21:57,480 --> 00:22:04,680
una cosa sería calcular a cómo va a quedar el dado, si calcular exactamente cómo le

237
00:22:04,680 --> 00:22:09,800
le pego al dado, como el dado de vuelta, como es toda su trayectoria hasta que cada rebota

238
00:22:09,840 --> 00:22:17,500
con el piso y sale una cara, que es yo la cara 5. Eso es una descripción determinista,

239
00:22:17,730 --> 00:22:22,160
que sería describir toda la trayectoria del dado. La descripción probabilística renuncia

240
00:22:22,700 --> 00:22:27,480
a hacer una descripción de la trayectoria completa y dice "bueno, solo me voy a contentar

241
00:22:27,480 --> 00:22:31,080
con dar la probabilidad de que sale a la cara 5.

242
00:22:31,870 --> 00:22:34,020
Es una lógica totalmente diferente.

243
00:22:35,250 --> 00:22:40,580
Sin embargo, también hay un formalismo matemático detrás de las probabilidades.

244
00:22:40,810 --> 00:22:44,220
Y eso es lo que vamos a intentar ver en estas clases.

245
00:22:45,240 --> 00:22:50,320
Tenga paciencia porque es una historia un tanto larga y llena de formulas.

246
00:22:51,360 --> 00:22:57,540
Bien, entonces, hay muchas formas diferentes de describir el formalismo cuántico.

247
00:22:58,780 --> 00:23:02,480
La más popular es la que utiliza espacios vectoriales o más,

248
00:23:03,140 --> 00:23:04,700
para hacer más preciso espacios de Hilbert.

249
00:23:05,940 --> 00:23:09,420
Entonces, lo que se hace es, por ejemplo,

250
00:23:10,000 --> 00:23:12,240
vieron que acá teníamos la partícula,

251
00:23:12,540 --> 00:23:14,680
podría pasar por la rendija izquierda a la derecha.

252
00:23:16,620 --> 00:23:20,160
Acá lo que tenemos es una distribución de probabilidad

253
00:23:20,200 --> 00:23:24,960
que corresponde a un patrón de interferencia. Para describir eso, por ahí en una primera

254
00:23:25,080 --> 00:23:32,720
aproximación, uno podría decir, bueno, te escribo si la partícula estuviera en la partícula,

255
00:23:32,750 --> 00:23:39,340
en la rendija izquierda, lo represento por un vector. Acá vamos a usar la anotación

256
00:23:40,720 --> 00:23:45,440
"ketz", después más adelante va a quedar claro que es esto, pero a los rectores lo

257
00:23:45,440 --> 00:23:53,280
vamos a denotar así. Y este vector lo vamos a representar por un vector de 2 coordenadas,

258
00:23:54,340 --> 00:23:59,740
coordenada 1 y coordenada 0. Ahora voy a explicar un poco más que es un espacio vectorial que son

259
00:23:59,820 --> 00:24:05,340
los vectors, vamos a discutir más de esto, pero el elemento matemático va a ser este.

260
00:24:07,880 --> 00:24:12,360
Y si la partícula está en la rendija derecha, lo representamos por otro vector.

261
00:24:14,660 --> 00:24:19,080
Si está en izquierda, ponemos el 1, 0 y si está en la derecha, usamos el vector 0, 1. Bien.

262
00:24:20,360 --> 00:24:25,060
Y entonces diría una descripción elemental de este experimento.

263
00:24:25,120 --> 00:24:28,880
Hay una descripción más compleja, obviamente más precisas,

264
00:24:28,980 --> 00:24:34,580
pero una descripción elemental de este experimento sería que a la salida de la primera pantalla,

265
00:24:35,290 --> 00:24:40,820
en el contexto de interferencia, la partícula se encuentra en un estado de superposición.

266
00:24:42,380 --> 00:24:46,220
Y ese estado de superposición se representa como una combinación lineal,

267
00:24:46,490 --> 00:24:48,040
ahora voy a explicar qué es combinación lineal,

268
00:24:48,320 --> 00:24:51,680
de los dos vectores que representan, respectivamente, a

269
00:24:52,060 --> 00:24:55,580
particular en la rendija izquierda y particular en la rendija derecha.

270
00:24:56,200 --> 00:25:01,240
Entonces, para entender esto y para poder entender algoritmos cuánticos,

271
00:25:01,380 --> 00:25:04,260
vamos a tener que aprender propiedades de los vectores,

272
00:25:04,520 --> 00:25:07,080
como se suman, como se multiplican por escalares,

273
00:25:07,660 --> 00:25:09,400
vamos a tener que aprender números complejos,

274
00:25:10,280 --> 00:25:13,760
y vamos a tener que aprender matrices y operadores niales.

275
00:25:15,900 --> 00:25:17,080
Bueno, ¿qué es un vector?

276
00:25:17,820 --> 00:25:20,120
Esto también en un momento en que sus vidas lo vienen,

277
00:25:21,900 --> 00:25:25,000
muy probablemente en la primaria, pero seguro en el secundario,

278
00:25:25,900 --> 00:25:29,140
pero no importa, lo vamos a tratar de refrescar acá al concepto.

279
00:25:30,360 --> 00:25:33,960
Para fijar ideas, piensen a un vector como una flecha,

280
00:25:34,420 --> 00:25:35,360
piensen en el plano, ¿no?

281
00:25:36,200 --> 00:25:39,740
El plano de siempre, el plano geométrico.

282
00:25:41,320 --> 00:25:47,880
En el plano ustedes pueden pensar en flechitas que tienen el origen en el centro de coordenadas

283
00:25:50,320 --> 00:25:58,320
y la punta en la cabecita de la flecha. Entonces bueno, ¿cómo sumamos geométricamente dos vectores?

284
00:25:58,700 --> 00:26:03,960
Bien, para sumarlos tengo que agarrar uno de los vectores por ejemplo el de arriba

285
00:26:04,500 --> 00:26:13,120
y primero trazo una paralela al segundo vector que corte a la cabecita del primer vector,

286
00:26:15,039 --> 00:26:21,800
trazo una recta que pase por la cabecita del vector de arriba que sea paralela al vector de

287
00:26:21,820 --> 00:26:36,080
y hago lo mismo con el vector de abajo, bien, típicamente esas dos, esas dos rectas se van a

288
00:26:36,100 --> 00:26:44,220
cortar en algún punto y ese punto va a ser la cabecita del vector suma, si el vector resultante

289
00:26:44,220 --> 00:26:50,180
de la suma va a ser el que tiene como origen el origen de los otros dos, el origen todo,

290
00:26:50,220 --> 00:26:54,880
vamos a hacer que todos tengan el mismo origen, el centro de coordenadas y la

291
00:26:54,920 --> 00:27:03,360
cabecita sea la punta de la flecha, entonces esa es la forma con reglas si quieren o escuadra,

292
00:27:03,640 --> 00:27:06,120
reglas de escuadra de sumar

293
00:27:09,140 --> 00:27:14,740
vectores, estos son ejemplos de vectores, estoy poniendo este ejemplo porque es un ejemplo que

294
00:27:14,880 --> 00:27:19,180
ustedes en teoría ya conocen o que al menos pueden visualizar si no conocían de antes,

295
00:27:20,000 --> 00:27:27,120
y dado un vector lo que podemos hacer es alargarlo por ejemplo si el vector tiene largo que sé yo

296
00:27:27,440 --> 00:27:33,980
uno lo puedo multiplicar por un escalar, lo puedo multiplicar por dos entonces construyo a partir

297
00:27:33,980 --> 00:27:41,600
del primer vector un vector que tiene la misma dirección y mismo sentido que el anterior pero

298
00:27:42,620 --> 00:27:48,060
tiene el doble de longitud y eso matemáticamente se representa por multiplicarlo por dos

299
00:27:48,060 --> 00:27:56,940
por ejemplo o por -1, si multiplico al vector original por -1 tengo un vector que tiene la

300
00:27:56,980 --> 00:28:02,940
misma dirección pero cambia el sentido y tiene la misma longitud y así siguiendo,

301
00:28:03,540 --> 00:28:10,140
ahora lo puedo multiplicar por un medio y cambio la longitud de la mitad y esto se puede pensar

302
00:28:10,220 --> 00:28:21,980
también como elementos de R2. ¿Qué es R2? Bueno, déjenme ir a la...

303
00:28:25,240 --> 00:28:25,840
al pizarro.

304
00:28:29,680 --> 00:28:34,920
Bueno, ustedes conocen los números reales, por ejemplo, conocen el 0, el 1, el 2,

305
00:28:35,460 --> 00:28:47,860
el 2,5, el p, el nº de, con ese al menos 5, el -4 tercios y así siguiendo.

306
00:28:48,740 --> 00:28:51,860
Entonces típicamente los números reales los representamos en una recta,

307
00:28:52,300 --> 00:28:58,580
que yo si este es el 1, el 0, y este es el 1, y este es el 2, y este es el 3 y así siguiendo,

308
00:28:59,760 --> 00:29:02,920
los puedo pensar como que están todos contenidos en una recta,

309
00:29:02,940 --> 00:29:05,460
y entonces por ejemplo los números fraccionarios

310
00:29:07,000 --> 00:29:10,540
puedo dar una representación geométrica sencilla por ejemplo el número

311
00:29:10,880 --> 00:29:20,560
humedio o del número cinco medios y también por ejemplo el número

312
00:29:20,660 --> 00:29:25,360
raíz de dos se puede representar porque si esto mide uno y esto mide uno usando

313
00:29:25,520 --> 00:29:32,260
pitágoras esto mide raíz de dos van con un compás y lo proyectan y tienen el

314
00:29:32,260 --> 00:29:39,860
número de 2, ya sí siguiendo, la idea es que los números que utilizan típicamente para

315
00:29:41,060 --> 00:29:47,340
calcular cuánta plata tiene en el banco, por ejemplo, se pueden agrupar en lo que se conoce como la

316
00:29:47,480 --> 00:29:59,260
recta de los números reales, es una recta, tienen que misalió una de R, es una R pintoreja, y ahora

317
00:29:59,260 --> 00:30:07,060
¿Qué pasa si en vez de un número dan dos números? Si ustedes quieren describir, por

318
00:30:07,120 --> 00:30:14,260
ejemplo, la posición de una partícula en el plano, pueden decir, bueno, quieren dar

319
00:30:14,280 --> 00:30:18,720
las coordenadas de este punto en el plano. A este llamamos eje x y a este lo llamamos

320
00:30:18,760 --> 00:30:30,560
Ej. Entonces por ejemplo este punto por ahí está en 3,2 en el eje x y en 1 en el eje y,

321
00:30:30,860 --> 00:30:40,460
sí, entonces lo que dan es un par, el par 3,2,1, sí, y ahí tienen un vector.

322
00:30:43,980 --> 00:30:47,300
Entonces, acá lo que estarían dando es,

323
00:30:49,220 --> 00:30:53,280
tiene una recta real horizontal y otra recta real vertical.

324
00:30:54,440 --> 00:30:57,360
Entonces lo que están dando es dos coordenadas en este caso.

325
00:30:58,210 --> 00:31:00,660
Y esto se conoce como R por R.

326
00:31:02,420 --> 00:31:04,320
O abreviado R2.

327
00:31:07,059 --> 00:31:12,800
R2 es importante para nosotros porque va a ser un ejemplo de espacio vectorial.

328
00:31:12,800 --> 00:31:20,580
pase del espacio vectorial real de dimensión 2. Entonces, para dar un número de R2 tenemos que dar

329
00:31:21,900 --> 00:31:30,060
dos coordenadas. Atención, en este curso a los vectores los vamos a representar como una columna

330
00:31:32,940 --> 00:31:40,280
y los vamos a representar así, B igual a, que soy yo, 1, 3. Esta va a ser la componente X y esta

331
00:31:40,280 --> 00:31:47,740
va a ser la componente "i". ¿Por qué los vamos a representar como vectores columna?

332
00:31:47,940 --> 00:31:54,460
Bueno, porque en cuántica es más cómodo trabajar así. No hay ningún motivo en realidad, porque

333
00:31:54,540 --> 00:32:00,040
podrían ser también vectores fila, no pasa nada. Se puede hacer todas las mismas cuentas

334
00:32:00,500 --> 00:32:08,360
cambiando filas por coluna. No pasa nada. Pero no importa. Para que todo se parezca más a lo que

335
00:32:08,360 --> 00:32:14,140
ustedes van a encontrar en los libros de cuántica, vamos a usar filas. Entonces, ¿cómo dibujamos este vector? Bueno,

336
00:32:15,990 --> 00:32:20,380
en el eje X ponemos 1, 1, y en el eje Y ponemos 1, 2, 3.

337
00:32:23,640 --> 00:32:26,140
Y me quedaría esta flechita de acá.

338
00:32:28,460 --> 00:32:29,320
Muy mal el dibujo.

339
00:32:32,620 --> 00:32:37,760
o por ejemplo, supongo que queremos representar el vector

340
00:32:41,040 --> 00:32:52,820
b igual a -2, 1, entonces tengo que ir a -2, -1, -2 en el eje x y a 1 en el eje y,

341
00:32:58,760 --> 00:33:06,540
Bien, y así siguiendo voy a tener vectores en el plano, también fíjense que podría dar no solo

342
00:33:07,180 --> 00:33:21,900
r2, podría considerar r por r por r, que sería r3 y un vector de r3 va a tener 3 coordenadas x y

343
00:33:21,900 --> 00:33:30,760
y Z, y eso si es un espacio real tiene una representación gráfica, acá doy la coordenada X,

344
00:33:32,420 --> 00:33:42,080
acá doy la coordenada Y y con la altura doy la coordenada Z y voy a tener representado

345
00:34:08,020 --> 00:34:09,419
¿Pregunt

346
00:34:12,080 --> 00:34:19,659
digamos que el x y que representa digamos la forma de la combinación lineal es 0 y 1

347
00:34:19,960 --> 00:34:25,540
si no estoy mal no sé si puede volver a esa página solo para comprar. Si lo voy a explicar

348
00:34:25,580 --> 00:34:35,280
de nuevo la verdad. Por ejemplo ahí en este caso tenes el vector 1 0 porque la coordenada

349
00:34:35,280 --> 00:34:37,480
x vale 1 y la coordenada y vale c

350
00:34:39,360 --> 00:34:42,040
después tenés por ejemplo acá cuando dice la superposition

351
00:34:43,419 --> 00:34:43,580
c

352
00:34:44,300 --> 00:34:45,580
cuando dice la superposition

353
00:34:46,399 --> 00:34:51,620
acá la coordenada x vale 1/2 y la coordenada y vale 1/2

354
00:34:52,080 --> 00:34:52,780
y así siguiendo

355
00:34:53,280 --> 00:34:55,679
ahora voy a decir como se suman los rectos de la fictoria

356
00:34:57,500 --> 00:35:04,860
Y ese 1 sobre el rey de 2 aparece por normalización, digamos lo así, aún no estoy seguro.

357
00:35:05,660 --> 00:35:13,900
En el caso cuántico sí, pero a este nivel estamos viendo vectores, yo todavía no estoy hablando de cuántica.

358
00:35:14,340 --> 00:35:19,280
Estoy comentando porque quiero transmitir la idea de un espacio vectorial.

359
00:35:19,870 --> 00:35:21,600
¿Qué va a ser un espacio vectorial?

360
00:35:22,280 --> 00:35:27,200
un conjunto de vectores, como los del plano, por ejemplo.

361
00:35:28,640 --> 00:35:33,980
Fíjate, en el plano XI puede tener infinitos vectores, en R2

362
00:35:34,400 --> 00:35:37,220
van a haber infinitos vectores, porque cada punto del plano

363
00:35:38,680 --> 00:35:42,500
define un posible vector, y cada punto del plano va a estar subcoordenado.

364
00:35:43,300 --> 00:35:47,260
Ahora, lo que les voy a mostrar es que esos vectores tienen ciertas propiedades,

365
00:35:47,420 --> 00:35:50,360
los puedo sumar, lo puedo multiplicar por escaladas, ven por ejemplo este,

366
00:35:50,780 --> 00:35:55,700
se multiplicaba por un medio o por dos o por menos uno o por lo que sea.

367
00:35:56,510 --> 00:36:01,740
Y los vectores se pueden sumar y se pueden multiplicar por escalares.

368
00:36:04,180 --> 00:36:04,320
Bien.

369
00:36:06,400 --> 00:36:14,280
Esa es como la idea de un espacio vectorial y por ahí esto parece muy tonto porque para

370
00:36:14,440 --> 00:36:16,140
muchos será chirreconocido.

371
00:36:16,540 --> 00:36:27,520
El problema es que en realidad una cuantica típicamente va a trabajar con espacios vectoriales que no son R3, R2, R, sí, va a trabajar con otro espacio.

372
00:36:27,750 --> 00:36:28,640
Ahora le voy a comentar.

373
00:36:29,380 --> 00:36:38,560
y así podrían tener R por R por RN veces y definir R a la N, ¿sí?

374
00:36:40,120 --> 00:36:59,000
y un V, un vector de N R a la N, esta E es como una Epsilon significa pertenece, este es el vector, vector pertenece a RN, ¿sí?

375
00:36:59,740 --> 00:37:12,080
un B que pertenece a Rn va a tener n componentes x1, x2, tata, tata, hasta xn, si estaban R3

376
00:37:12,140 --> 00:37:15,520
tenia 3 componentes, si estaban R2 tiene 2 componentes, se entiende?

377
00:37:16,240 --> 00:37:17,520
y así va a tener Rn

378
00:37:20,160 --> 00:37:27,260
fíjense algo interesante, ustedes pueden visualizar R2 y R3, porque pueden

379
00:37:27,260 --> 00:37:35,640
tener una representación visual ya sea en el plano o en el espacio tridimensional.

380
00:37:36,840 --> 00:37:44,640
Típicamente R2 y R3 se pueden utilizar para modelar posiciones en un plano o en el espacio

381
00:37:44,740 --> 00:37:53,860
tridimensional, pero ya R4 no tiene una descripción visual, o R5 o R6 son entes puramente matemáticos,

382
00:37:53,900 --> 00:38:00,540
si quieren, o al menos no tienen la representación intuitiva visual, bien,

383
00:38:02,940 --> 00:38:09,140
bien, y qué va a pasar, qué va a pasar, yo les dije antes que podían sumar

384
00:38:09,220 --> 00:38:15,440
vectores, entonces si tenían que ser un vector así y otro vector a z,

385
00:38:16,859 --> 00:38:22,539
trazabanla para la una, y tenían el vector suma, y eso tenía un

386
00:38:22,540 --> 00:38:29,020
relato geométrico. Resulta hacer que lo que termina pasando es que si ustedes tienen que yo

387
00:38:29,200 --> 00:38:42,340
b1 igual a 1, 2 y b2 igual a, no sé, 3, 4, tienen los números al hacer, ¿no? Hacer esta suma con que

388
00:38:42,720 --> 00:38:48,340
esta ley de la suma se llama ley del paralelogramo porque para construir la resultante de la suma

389
00:38:48,340 --> 00:38:57,180
arman un paralelogramo, resulta que la suma del paralelogramo coincide con sumar coordenada

390
00:38:57,240 --> 00:39:05,480
coordenada, entonces tengo b1, tengo b2 hago b1 + b2 y eso es poner 1, 2 + 3, 4

391
00:39:10,020 --> 00:39:15,740
y acá la resultante de la suma tiene que hacer coordenada coordenada, es decir la primera de

392
00:39:15,740 --> 00:39:22,480
este se suma con la primera y la segunda con la segunda, entonces queda 1 + 3 y 2 + 4

393
00:39:24,960 --> 00:39:27,240
y esto queda como 4 y 6

394
00:39:33,880 --> 00:39:39,540
y si tienen que sumar por ejemplo vectores de R3 es muy parecido por ejemplo si tienen

395
00:39:39,580 --> 00:40:09,560
p1 igual a 1, 2, 3 y b2 igual a -1, -2 y 4, entonces la suma de b1 más b2 es 1, 2, 3 más -1, -2, -2, 4

396
00:40:11,579 --> 00:40:19,960
lo hago lento por las dos, uno más menos uno en la primera, dos más menos dos en la segunda y después

397
00:40:20,620 --> 00:40:26,780
tres más cuatro en la tercera y esto queda cero cero y siete.

398
00:40:31,440 --> 00:40:35,840
Y la otra cosa que les decía era que si uno tenía un vector por ejemplo,

399
00:40:37,860 --> 00:40:40,800
el vector 2 1

400
00:40:45,360 --> 00:40:46,380
el vector 2 1

401
00:40:49,350 --> 00:40:53,020
y si hacemos 2 por el vector 2 1

402
00:40:53,690 --> 00:40:58,500
se me alargaba por 2, entonces 2 por B es 2 por 2 1

403
00:41:00,720 --> 00:41:01,240
y esto es

404
00:41:03,060 --> 00:41:07,480
el 2 tiene que multiplicar a cada una de las componentes, 2 por 2 y 2 por 1

405
00:41:09,120 --> 00:41:13,580
y esto es 4, 1, entonces no, 4, 2 por 1

406
00:41:18,480 --> 00:41:19,280
entonces el...

407
00:41:21,740 --> 00:41:23,000
pasa al 4, 2, ¿sí?

408
00:41:24,440 --> 00:41:25,900
¿Qué quiero decir con este ejemplo?

409
00:41:26,420 --> 00:41:31,300
Que multiplicar por números reales o sumar vectores

410
00:41:31,370 --> 00:41:34,240
se corresponde con las operaciones geométricas

411
00:41:34,480 --> 00:41:36,940
de alargar o chicar vectores o cambiarles el sentido

412
00:41:37,920 --> 00:41:40,860
y sumar de acuerdo a la regla del paralegrogramo.

413
00:41:41,350 --> 00:41:42,440
¿Y cómo es la suma?

414
00:41:42,780 --> 00:41:44,020
Bueno, coordenada, coordenada.

415
00:41:44,150 --> 00:41:52,280
Si tengo, por ejemplo, un B que es B1, B2, ¿no?

416
00:41:53,440 --> 00:42:10,540
un W que es W1 W2, la suma de W, se define como W1 + W1 y W2 + W2, así se suman los rectores,

417
00:42:11,490 --> 00:42:19,680
acá puse un ejemplo en R2, bueno en R3 y en R4 y en Rn es lo mismo, si tengo en Rn

418
00:42:21,740 --> 00:42:35,240
un B que es V1, V2 hasta Vn, y tenemos un W que es W1 hasta Wn.

419
00:42:38,960 --> 00:42:52,200
la suma y de B+WB es B1+WB1, B2+WB2 y así siendo BN+WBN.

420
00:42:54,040 --> 00:42:54,180
Bien.

421
00:42:59,060 --> 00:43:01,220
Bueno, se entiende hasta acá.

422
00:43:04,320 --> 00:43:15,360
de la misma manera la escala de alfa por b sería alfa por b1 alfa por b2 alfa por bn

423
00:43:19,160 --> 00:43:23,500
voy a darse preguntas en el chat o si solo le dijeron que sí

424
00:43:26,620 --> 00:43:28,500
sí sí sí bien

425
00:43:29,600 --> 00:43:30,520
bueno alguna pregunta

426
00:43:34,500 --> 00:43:43,600
bien, bien, entonces ahora lo que es muy importante es abstraer todo esto, abstraer y capturar

427
00:43:43,600 --> 00:43:49,360
la noción del espacio vectorial, ¿eh? porque bueno, ¿qué va a ser un espacio vectorial?

428
00:43:51,320 --> 00:43:59,600
un espacio vectorial sobre los números reales va a ser un conjunto B, acá sería cada punto

429
00:43:59,600 --> 00:44:07,700
del cada punto posible del plano, por ejemplo si están en R2 sería un vector y el conjunto

430
00:44:07,830 --> 00:44:13,200
de todos los vectores sería el espacio vectorial, entonces va a ser un conjunto no vacío que

431
00:44:13,200 --> 00:44:19,100
va a estar dotado una suma si tiene un concepto de suma de vectores y un producto por escalares

432
00:44:19,460 --> 00:44:26,700
como el que hay que sacar por 2, por 3, por -5 o por lo que sea, con las siguientes propiedades.

433
00:44:27,400 --> 00:44:36,860
primer lugar la suma es asociativa, es decir, B se ha o el resultado de hacer B más B más

434
00:44:37,020 --> 00:44:47,260
W es lo que vamos a hacer, B más W más W. Esto podría parecer obvio con números reales

435
00:44:47,320 --> 00:44:55,220
pero no está novio con vectores, hay operaciones por ejemplo el producto cruise que no va,

436
00:44:55,460 --> 00:45:04,920
un cruz, un nuevo gordo. Hay operaciones algebraicas que no son asociativas, por ejemplo, pero en este caso

437
00:45:05,430 --> 00:45:12,260
la suma de espacios vectoriales es asociativa. Es computativa también, da lo mismo hacer b+w+b,

438
00:45:12,260 --> 00:45:19,780
que w+b, el resultado es el mismo. Hay un neutro para la suma, hay un vector que es nulo, en qué

439
00:45:19,780 --> 00:45:28,120
sentido que se hacen b+0 es 0+b y eso es igual a b, es decir es un vector que tiene la propiedad de que

440
00:45:28,180 --> 00:45:36,300
no cambia la suma, ¿cuál es ese vector? El vector nulo es el que tiene todos 0,

441
00:45:41,040 --> 00:45:45,800
entonces hacen b+0 es b siempre, ok?

442
00:45:50,540 --> 00:45:51,060
bien

443
00:45:55,599 --> 00:45:59,580
y para fijar ideas también, si están en R3

444
00:46:02,780 --> 00:46:03,380
el 0

445
00:46:06,740 --> 00:46:11,300
es el que tiene x y y z igual a 0, ese es el punto que está en el centro,

446
00:46:12,880 --> 00:46:16,700
en el centro de coordenados, el 0,0,0

447
00:46:18,320 --> 00:46:21,940
y de mismo modo tiene el 0 de RLINE

448
00:46:24,360 --> 00:46:27,420
después otra cosa importante es que para todo B existe un B'

449
00:46:28,100 --> 00:46:29,800
tal que B más B' es igual a 0

450
00:46:30,680 --> 00:46:31,480
¿Qué quiere decir esto?

451
00:46:31,490 --> 00:46:34,640
bueno, que la suma tiene un inverso, desadelanto

452
00:46:35,560 --> 00:46:37,300
o al menos ya lo puede intuir

453
00:46:37,450 --> 00:46:42,860
el resultado es que B' es menos B

454
00:46:42,860 --> 00:46:46,580
más -1 por b, esto se igual a 0,

455
00:46:48,580 --> 00:46:52,480
que sería b más -b, lo voy a hacer.

456
00:46:53,900 --> 00:47:00,040
Y por qué es así? Bueno, porque si b es b1 hasta b,

457
00:47:06,860 --> 00:47:21,600
-b es, tengo que multiplicar a todos por -1, queda -b1, -b2, -bn, entonces cuando lo sume se va a cancelar

458
00:47:21,680 --> 00:47:33,380
coordenada, coordenada y me va a quedar el vector que tiene todos ceros. Después también, dados dos

459
00:47:33,380 --> 00:47:40,980
números reales y cualquier vector es lo mismo primero multiplicar el vector por

460
00:47:41,140 --> 00:47:46,260
b por b larga y después a ese nuevo vector multiplicarlo por a que hacer

461
00:47:46,380 --> 00:47:50,960
primero a por b larga y a ese número multiplicarlo por b

462
00:47:52,760 --> 00:47:58,260
básicamente estas operaciones quieren decir que tienen que hacer lo que

463
00:47:58,260 --> 00:48:05,800
algo muy parecido a lo que pasa con los números reales. El 1 es el, si multiplica un vector por 1,

464
00:48:06,120 --> 00:48:17,060
no cambia nada, queda igual. Y esto es importante, que sería como una propiedad de linealidad. Si sumo

465
00:48:17,080 --> 00:48:22,540
dos vectores y los multiplico por un número que es yo por 2, por 3, por lo que sea, eso es lo

466
00:48:22,540 --> 00:48:27,320
mismo que multiplicar a cada uno de los dos vectores por separado y después sumarlos,

467
00:48:27,690 --> 00:48:34,660
es decir, la resultante es el mismo vector. Y después para cualquier número a y b reales

468
00:48:34,780 --> 00:48:40,580
para todo vector es lo mismo hacer a + b sumar los números y a ese número multiplicarlo por

469
00:48:40,660 --> 00:48:47,440
el vector que multiplicar al vector por cada uno de los números y después sumar los vectores.

470
00:48:48,320 --> 00:48:53,940
Entonces estas son las propiedades que definen a lo que se conoce como un espacio vectorial.

471
00:48:56,220 --> 00:49:03,140
Entonces ¿Qué es un espacio vectorial? Es un conjunto que tiene una noción de suma,

472
00:49:03,250 --> 00:49:07,920
una operación de suma y una operación de producto por números reales en este caso,

473
00:49:08,060 --> 00:49:13,800
porque en este caso estaríamos tratando con un espacio vectorial real y que tiene estas

474
00:49:13,800 --> 00:49:21,620
propiedades. Cualquier entidad que cumple con esto se puede llamar espacio

475
00:49:21,720 --> 00:49:25,520
editorial sobre los números reales. ¿Por qué esto no es evidente? Porque ustedes me

476
00:49:25,600 --> 00:49:28,360
dicen "che, bueno, pero fe, qué voludes, tanto quilombo"

477
00:49:30,580 --> 00:49:36,280
Si queda claro, R2 es obvio que se cumplen estas cosas, no? en Rn lo acabamos de ver,

478
00:49:36,440 --> 00:49:41,760
¿no? porque en el fondo gran parte de estas propiedades se heredan de los

479
00:49:41,760 --> 00:49:45,300
números reales porque la suma de vectores y la multiplicación por escalares es

480
00:49:45,360 --> 00:49:49,820
coordenada, coordenada. Entonces en el fondo Rn va a tener

481
00:49:51,119 --> 00:49:55,960
variadas esas propiedades. Bien, no es trivial porque uno puede tener espacios

482
00:49:56,060 --> 00:50:01,500
vectoriales de cosas que no sean los vectores de R2. Por ejemplo, por ejemplo,

483
00:50:02,220 --> 00:50:08,200
uno podría tener un espacio vectorial complejo, un espacio vectorial sobre los

484
00:50:08,200 --> 00:50:14,080
número complejo, se suma un conjunto no vacío que tiene una suma y producto y un concepto

485
00:50:14,220 --> 00:50:17,800
de multiplicación por números complejos con las siguientes propiedades, ¿cuáles

486
00:50:17,900 --> 00:50:25,240
las mismas? Pero ahora, ¿quieren números complejos? Y las componentes son también números complejos.

487
00:50:25,330 --> 00:50:32,120
Por ejemplo, vamos a ver. Primero, ¿qué es un número complejo? Eso también es importante,

488
00:50:32,960 --> 00:50:38,760
este curso es súper, súper importante que repasen las propiedades de los números complejos.

489
00:50:39,700 --> 00:50:47,080
Vamos a ver un poquito esto. Los números complejos tienen que ver con,

490
00:50:52,640 --> 00:50:53,360
con este problema.

491
00:50:57,320 --> 00:51:01,840
Si concebamos la ecuación x cuadrado menos 1 igual a 0 y les digo, bueno,

492
00:51:01,960 --> 00:51:07,880
busquen las raíces de esta ecuación, las soluciones de esta ecuación, entonces esto les queda x cuadrado igual a 1,

493
00:51:08,160 --> 00:51:17,080
paso restando el 1, lo paso sumando y cuando saco la raíz cuadrada me queda x igual a 1 y x igual a -1,

494
00:51:18,660 --> 00:51:24,140
eso son las raíces, pero qué pasa si pregunto por las soluciones de x cuadrado más 1 igual a 0,

495
00:51:26,200 --> 00:51:34,180
pregunta, hay un número que cuando le sume algo, que cuando le le va al cuadrado y le sume uno me de 0

496
00:51:37,240 --> 00:51:41,960
a priori no, no porque si busco en la recta de los números reales

497
00:51:44,340 --> 00:51:49,580
si el número es positivo, si es 0 listo, no es solución porque me queda 1 y 1 no es 0 listo,

498
00:51:49,580 --> 00:51:56,900
0 no es solución, si el número es positivo, x, 1 más algo positivo me queda más grande que 1, eso tampoco es 0

499
00:51:57,800 --> 00:52:03,300
y si es negativo, si es un número negativo que yo el -5, y hago -5 al cuadrado más 1

500
00:52:04,520 --> 00:52:13,580
siempre cuando le da al cuadrado el -5, el - se va por -5 por -5, menos por menos es más, me queda 25

501
00:52:13,580 --> 00:52:16,400
Esto queda 26, esto es distinto de 0.

502
00:52:16,540 --> 00:52:19,400
Entonces eso va a pasar siempre, siempre, siempre, siempre.

503
00:52:20,200 --> 00:52:22,660
Esto no tiene solución en los números reales.

504
00:52:23,940 --> 00:52:25,300
Verán que creo que no hay un pregunto algo.

505
00:52:27,500 --> 00:52:29,160
Claro, exacto, raíz de menos 1.

506
00:52:29,240 --> 00:52:32,100
Entonces la pregunta es, ¿existe raíz de menos 1?

507
00:52:32,340 --> 00:52:34,760
Bien, en los números reales no hay raíz de menos 1.

508
00:52:36,280 --> 00:52:42,100
Pero uno puede inventar unos números que sean solución de

509
00:52:42,100 --> 00:52:56,300
ecuación y decir que las soluciones son y y -y y que es y? y es un número tal que al cuadrado es igual a

510
00:52:56,320 --> 00:53:01,060
menos 1, es el número imaginario

511
00:53:05,440 --> 00:53:10,320
bueno, ahora la representación gráfica sencilla de los números complejos, ahora lo voy a decir,

512
00:53:10,380 --> 00:53:26,980
pero antes déjame comentar esto, entonces, whiteboard, entonces inventamos un número, un número nuevo

513
00:53:27,540 --> 00:53:33,160
que no estaba antes en la recta real, tenemos la recta real, el 0, etcétera, bueno y no está acá,

514
00:53:33,560 --> 00:53:38,700
no es ningún punto en la recta real, es un número que al cuadrado da menos uno, ningún número real

515
00:53:38,700 --> 00:53:44,900
puede hacer eso bien, pues un número complejo en general se va a expirir así como a + b por y

516
00:53:49,160 --> 00:53:56,020
donde a y b pertenecen a los reales, a y b son números reales, que quiere decir que a y b son

517
00:53:56,120 --> 00:54:00,760
números que sí se pueden representar en la recta pero y no, ¿está bien?

518
00:54:03,820 --> 00:54:09,920
Entonces, ¿cómo se suman los números complejos?

519
00:54:10,280 --> 00:54:18,980
La idea es que se sumen igual que antes, si tengo z igual a a + b por i

520
00:54:19,830 --> 00:54:30,820
y tengo w igual a c + d por i, entonces z + w va a ser a + c

521
00:54:32,320 --> 00:54:35,140
y después hago B por I más D por I.

522
00:54:36,260 --> 00:54:43,620
Al número I lo trato como cualquier otro número y lo saco factor común, entonces me queda Amac + B + D por I.

523
00:54:45,280 --> 00:54:54,980
Yo podría definir suma de números complejos de esta manera, decir que I es el número que al cuadrado da -1 y que la suma se define así.

524
00:54:55,820 --> 00:54:59,220
Pero como regla nemotécnica es siempre bueno hacer esta sublita.

525
00:54:59,620 --> 00:55:01,700
Tratar el número "i" como si fuera un número más,

526
00:55:03,080 --> 00:55:05,800
solo teniendo en cuenta que "i" cuadrado de -1.

527
00:55:06,070 --> 00:55:08,060
Y también pueden definir la multiplicación,

528
00:55:08,660 --> 00:55:13,720
como pueden motivar la multiplicación de números complejos así.

529
00:55:15,000 --> 00:55:19,660
Z por Wb es a + b por i por c + d por i.

530
00:55:20,400 --> 00:55:21,860
Entonces ahora hacen todos contra todos.

531
00:55:22,740 --> 00:55:38,080
esta sería A por C, después más A por D por I, más B por I por C más B por D por I, por I,

532
00:55:39,100 --> 00:55:46,800
ven que multipliqué, todos contra todos, si sea distributivo, bien, ya tengo A por C, fíjense, I por I,

533
00:55:48,260 --> 00:55:51,800
y por "y" es igual a "y" cuadrado y esto es igual a -1

534
00:55:57,280 --> 00:56:02,500
Entonces este término que tiene "y" cuadrado me queda menos "re" por "d" en realidad

535
00:56:06,920 --> 00:56:09,960
¿Por qué no me le borra?

536
00:56:11,220 --> 00:56:12,260
Con el control "z"

537
00:56:15,260 --> 00:56:19,280
me cago, no se, esperen que voy a borrar

538
00:56:29,339 --> 00:56:38,200
menos b por d y después a este i lo sacan factor común y les queda a por d más b por c

539
00:56:38,360 --> 00:56:44,800
todo por "y". Entonces pueden definir z por w, así.

540
00:56:52,500 --> 00:56:59,240
Se escriben así como un algo real más algo real por "y" y que se suman y multiplican de acuerdo

541
00:56:59,340 --> 00:57:06,860
a estas ecuaciones que les puse acá. Y eso ya define lo que se conoce como "c", el campo de

542
00:57:06,860 --> 00:57:14,900
los números complejos. Bueno, este campo es súper crucial en cuántica porque en cuántica no

543
00:57:15,000 --> 00:57:20,880
vamos a usar espacios vectoriales reales, sino que vamos a usar espacios vectoriales complejos.

544
00:57:22,450 --> 00:57:30,140
Esto es el mensaje crucial de la clase de hoy. Entonces, así como en física clásica teníamos

545
00:57:30,260 --> 00:57:39,700
R2 que es la energía de un sistema, la representamos como un número real. La posición en el plano

546
00:57:40,260 --> 00:57:51,240
como un número en R2 y la posición en el espacio de euclidio como un punto en R3. Bien, en cuántica

547
00:57:51,260 --> 00:58:01,900
vamos a tener C, C2, C3, C4 y así hasta C a la n. La gracia es que el espacio de qubits,

548
00:58:03,660 --> 00:58:09,640
el espacio de estado de una computadora cuántica va a ser representado por un vector en C a la n.

549
00:58:16,480 --> 00:58:23,300
va a ser un alfa 1, alfa 2, alfa n, donde los alfa y son números complejos.

550
00:58:23,680 --> 00:58:29,700
Si tienen el mensaje del día y lo que tienen que entender cuando van los

551
00:58:29,920 --> 00:58:37,140
ejercicios y le dan los libros en casa. El espacio de estados cuánticos va a

552
00:58:37,180 --> 00:58:42,500
hacer alguno de estos, en el caso de la computación cuántica, algún c a la n para

553
00:58:42,500 --> 00:58:51,720
un n. Ahora voy a seguir sobre esto. Bien, me preguntaban antes dónde está Ali, cuál es la representación

554
00:58:51,820 --> 00:58:58,980
geométrica. Bueno, hay una representación geométrica de los complejos sencillas que es. Si uno pone z como

555
00:58:59,200 --> 00:59:09,260
a + b + y esto lo puede ver como dos coordenadas reales. Pienso a Ali, a lo que multiplica al número

556
00:59:09,260 --> 00:59:17,800
imaginaria como la componente imaginaria y eso tiene un nombre re de z es igual a a que es la

557
00:59:17,840 --> 00:59:28,420
parte real e in de z es igual a b que es la componente imaginaria hay un chiste que es muy tonto de

558
00:59:28,910 --> 00:59:36,700
no sé se la van pasando profesores este por generaciones de profesores yo lo aprendí en cdc

559
00:59:36,700 --> 00:59:44,140
cuando cursaba y es mi vida sexual es muy compleja tiene una parte real muy pequeña y una parte

560
00:59:44,240 --> 00:59:49,440
imaginaria muy grande es un chiste muy estúpido pero yo cumplo en transmitirse los ustedes cuando

561
00:59:49,700 --> 00:59:55,480
sean docentes se lo van a transmitir a sus alumnos y a quedar con unos boludos pero bueno

562
00:59:57,500 --> 01:00:00,260
como como ven un número un

563
01:00:02,380 --> 01:00:06,380
Un número complejo lo pueden pensar como un vector de dos componentes entonces

564
01:00:07,400 --> 01:00:13,860
este va a ser el eje real y este va a ser el eje imaginario entonces vos me preguntabas cómo

565
01:00:13,960 --> 01:00:22,320
represento al número y bueno acá ahora este es el plano complejo se entiende es distinto como

566
01:00:22,380 --> 01:00:26,019
espacio no es r2 porque vamos a tratar de pensar eso

567
01:00:29,060 --> 01:00:34,980
A nivel conjunto son lo mismo, son biyectivos porque para cada número complejo

568
01:00:35,480 --> 01:00:39,580
puede encontrar un par de números reales y vice-barza, tengo una asignación uno a uno.

569
01:00:40,020 --> 01:00:45,600
Es como tener una aula llena de estudiantes sentados, hay la misma cantidad de sillas que de estudiantes.

570
01:00:46,280 --> 01:00:55,600
Hay la misma cantidad de números complejos que de puntos en el plano.

571
01:00:56,500 --> 01:01:06,600
Sin embargo, R2 es diferente como conjunto porque tiene una suma y una multiplicación por escalares que no es la misma.

572
01:01:07,030 --> 01:01:11,760
Esta suma de acá en un número real es no es la misma que la suma del número en los complejos.

573
01:01:11,760 --> 01:01:14,280
Bueno, sí, pero la suma es la misma.

574
01:01:14,780 --> 01:01:15,660
Perdón, perdón, perdón.

575
01:01:15,660 --> 01:01:15,920
Me quedo aquí.

576
01:01:16,630 --> 01:01:17,340
La suma es la misma.

577
01:01:17,950 --> 01:01:19,320
La multiplicación por la escala es también.

578
01:01:20,140 --> 01:01:24,200
Pero lo que cambia es que el producto,

579
01:01:25,020 --> 01:01:27,260
ustedes no hacen producto de números reales,

580
01:01:27,600 --> 01:01:29,340
de puntos del plano.

581
01:01:29,800 --> 01:01:31,720
Hay productos de puntos del plano que los vamos

582
01:01:31,730 --> 01:01:33,620
a usar después, más adelante.

583
01:01:34,780 --> 01:01:38,040
Pero esta operación de acá no está en arreglos.

584
01:01:40,200 --> 01:01:47,560
estas z por w típicamente no la hacen en los redes, entonces eso los distingue algebraicamente

585
01:01:51,160 --> 01:01:55,860
pero bueno para nosotros no sé si hay hay matemáticos en la sala

586
01:01:58,700 --> 01:02:00,500
si hay ahí listo

587
01:02:02,700 --> 01:02:11,780
No podemos decir barras basadas, pero para los que no entiendan nada de matemática es parecido.

588
01:02:12,320 --> 01:02:18,560
Se puede pensar a los complejos como puntos de perro, pero no los son porque las opresiones algeóricas son diferentes.

589
01:02:19,540 --> 01:02:27,920
No es el mismo concepto matemático y de hecho los complejos son un cuerpo.

590
01:02:28,920 --> 01:02:35,040
Por eso los complejos se piensan como escalares cuando definimos a los espacios vectoriales complejos.

591
01:02:35,950 --> 01:02:37,320
Este es el que nos van por tener en cuenta.

592
01:02:38,480 --> 01:02:42,100
Entonces el espacio vectorial sobre los números complejos es un conjunto B,

593
01:02:43,000 --> 01:02:47,900
una vació que tiene una suma y un producto por números complejos con las siguientes propiedades.

594
01:02:47,950 --> 01:02:50,320
Y las propiedades son muy parecidas a las anteriores,

595
01:02:51,560 --> 01:02:53,500
nada más que ahora tenemos números complejos.

596
01:02:53,600 --> 01:03:21,300
Entonces bueno, si una hora considera, considera a los, a sea la n por ejemplo, c2, consideramos c2, serían los vectores que tienen dos coordenadas complejas y bueno,

597
01:03:23,420 --> 01:03:28,560
si tengo un W que es gama delta

598
01:03:31,040 --> 01:03:35,460
B+W va a ser alpha + gama y beta + delta

599
01:03:37,360 --> 01:03:43,500
donde ahora alfa, beta, gama y delta son números complejos

600
01:03:46,040 --> 01:03:50,600
fíjense que hay una diferencia entre

601
01:03:51,200 --> 01:03:54,400
hay alguien que tiene el micrófono prendido por favor, a par

602
01:03:54,700 --> 01:03:55,200
yo disculpe

603
01:03:56,120 --> 01:03:59,260
si, C2 es bastante distinto de R2, por qué?

604
01:04:00,300 --> 01:04:05,340
porque R2, un vector de R2 tiene dos coordenadas reales

605
01:04:06,660 --> 01:04:12,300
mientras que un vector de C2 tiene un Z y un W

606
01:04:14,020 --> 01:04:15,680
tiene dos coordenadas complejas

607
01:04:16,380 --> 01:04:26,100
y cada uno de estos tiene dos números reales. Entonces, para definir un vector en c2 tienen

608
01:04:26,100 --> 01:04:29,660
que dar cuatro números reales, mientras que para definir un vector en r2 tienen que dar

609
01:04:29,760 --> 01:04:37,480
dos números reales, ya estos son bastante diferentes entre sí. Pero la suma, la multiplicación

610
01:04:37,520 --> 01:04:42,600
por escalares es todo igual, todo igual. Yo preparé unos ejercicios que después son

611
01:04:42,600 --> 01:04:47,320
muy sencillo de todas formas, después voy a subir a la plataforma de la materia para que ustedes

612
01:04:47,380 --> 01:04:55,780
practiquen sumas de doctores complejos, que es ello, multiplicación por escalares. Entonces hago un ejemplo

613
01:04:55,880 --> 01:05:18,020
por ejemplo, supongamos que tenemos b igual a -i y 3 + 2i y que w es igual a 2i y -1 + 4i

614
01:05:19,560 --> 01:05:22,540
Bueno, ¿cómo sería hacer 3 por B?

615
01:05:23,940 --> 01:05:27,880
Entonces, hacer 3 por -i y 3 más 2i.

616
01:05:29,020 --> 01:05:31,480
El 3 multiplica componente a componente,

617
01:05:31,700 --> 01:05:37,140
entonces queda 3 por -i y 3 por 3 más 2i.

618
01:05:38,340 --> 01:05:39,980
Sido a la derecha.

619
01:05:45,220 --> 01:05:50,120
y acá me quedan -3*i y 3*39 + 3*26i

620
01:05:52,020 --> 01:06:00,160
o podrían hacer por ejemplo, pueden hacer, piensen acá definir no, b y w arriba

621
01:06:00,420 --> 01:06:07,300
entonces voy a hacer 2*b -i*w

622
01:06:09,220 --> 01:06:14,740
entonces tengo que hacer 2 por -1 y 3 más 2 y

623
01:06:16,580 --> 01:06:22,100
menos y por 2 y y menos 1 más 4 y

624
01:06:30,100 --> 01:06:37,840
Entonces 2 por menos y es -2y y tengo que hacer 6 más 4y.

625
01:06:41,020 --> 01:06:48,620
Y después ahora tengo que hacer más el -y lo meto acá dentro, me queda -y por 2y es

626
01:06:49,560 --> 01:06:52,020
por menos y por 2y

627
01:06:53,620 --> 01:06:57,320
y después menos y por menos 1 más 4y

628
01:07:03,020 --> 01:07:06,800
el próximo paso me queda menos 2y y después 6 más 4y

629
01:07:08,120 --> 01:07:08,640
pues más

630
01:07:10,360 --> 01:07:14,380
y por 10 menos 1 menos por menos más, acá me quedan 2 y después me queda

631
01:07:15,360 --> 01:07:19,500
más y y menos 4, menos 4 más y

632
01:07:22,280 --> 01:07:26,260
y por último me queda menos, me queda 2 menos 2 y

633
01:07:27,440 --> 01:07:32,540
y después 2 más 5 y

634
01:07:33,880 --> 01:07:36,820
pero que voy haciendo acá sumé coordenada, coordenada

635
01:07:38,440 --> 01:07:42,960
y este complejo más este complejo, este complejo más este complejo le puse acá

636
01:07:43,460 --> 01:07:48,280
pregunta me siguieron en esto o no cómo vienen con esto se entiende no se

637
01:07:48,340 --> 01:07:53,580
entiende nada no los estoy jugando necesito saber si entienden no

638
01:07:53,740 --> 01:08:01,280
entienden a mi falta practicarlo pero sí sí bueno para mí es muy importante

639
01:08:01,900 --> 01:08:08,940
saber si no entienden nada si alguien no entiende nada por favor mande me mail o

640
01:08:08,940 --> 01:08:15,940
WhatsApp, y saben que no entienden nada porque así yo voy buscando herramientas pedológicas

641
01:08:16,009 --> 01:08:21,660
y diseñando ejercicios para ver si, claro, bueno, claro, ok.

642
01:08:22,339 --> 01:08:30,200
Bien, ¿qué pasa con esto? ¿Y cuál es uno de los grandes desafíos de un curso como

643
01:08:30,279 --> 01:08:37,820
este? Bien, alguien como yo o como Juan están por ahí dos años haciendo estas cuantitas

644
01:08:37,819 --> 01:08:41,100
porque ven al georanial primero en el CVC, en la UBA,

645
01:08:41,240 --> 01:08:46,480
si, en la UBA, después por ahí ven al georanial dos veces más en la carrera,

646
01:08:46,540 --> 01:08:47,799
después le vuelven a ver las materias.

647
01:08:47,850 --> 01:08:50,580
Entonces uno está años haciendo, yo debo hacer 25 años,

648
01:08:50,670 --> 01:08:52,839
veo al georanial, porque hago física, cuántica.

649
01:08:54,300 --> 01:08:57,240
Pero hay gente que por ahí viene de informática

650
01:08:57,460 --> 01:09:00,600
y lo ve en una materia una vez y ya se olvidó.

651
01:09:01,160 --> 01:09:04,180
Ya se olvidaron, lo ve, lo ve hace cinco años, se acuerdan de nada.

652
01:09:05,080 --> 01:09:06,259
O hay gente que por ahí no lo ve nunca.

653
01:09:07,020 --> 01:09:13,759
Yo se los estoy dando todo de cero, pero la realidad es que el contenido de un curso,

654
01:09:15,100 --> 01:09:21,640
si ustedes no practican y no leen libros, no alcanzan para que tengan fluidez en estas manipulaciones al georécas, sí.

655
01:09:22,340 --> 01:09:29,520
Yo lo puedo hacer muy rápido y por ahí no sé, Juan, lo puedo hacer muy rápido porque hace años que estamos con esto,

656
01:09:29,660 --> 01:09:33,960
pero aquí no está en tema, le cuesta la operatoria al georéc.

657
01:09:34,020 --> 01:09:41,000
Entonces mi invitación es que hagan ejercicios y que se pongan a leer los libros que les voy a hacer,

658
01:09:41,390 --> 01:09:43,980
a leerlos meticulosamente, es muy importante.

659
01:09:44,650 --> 01:09:46,440
Y que lo que no entiendan lo pregunten.

660
01:09:47,180 --> 01:09:48,600
Se lo pueden, es como el padre.

661
01:09:50,020 --> 01:09:53,700
Claro, exacto, multiplicar partidos, ya ni pensás cuando lo haces.

662
01:09:53,900 --> 01:09:58,860
Viste conceptos que ya están grabados en célebros, que uno no piensa...

663
01:09:59,980 --> 01:10:01,860
Sí, uno está automatizado, exacto.

664
01:10:02,660 --> 01:10:14,440
Exactamente. Pero bueno, quienes sientan que esto es difícil, piensen primero, no es tan difícil y segundo, es importante que tengan una segunda instancia.

665
01:10:14,760 --> 01:10:21,380
Aparte de la clase, tienen que sentarse en un horario extra a leer el libro y a tratar de hacer ejercicios.

666
01:10:21,720 --> 01:10:27,940
En particular, yo les voy a dar para que dan los ejercicios del libro Daniel Zenichuan.

667
01:10:28,260 --> 01:10:30,620
Sí, es importante que intenten hacerlo.

668
01:10:31,720 --> 01:10:35,320
También, otra cosa que Juan sabe y que yo sé y que los físicos sabemos,

669
01:10:35,520 --> 01:10:38,880
pero que el resto por ahí no lo sabe, es que esto cuesta mucho.

670
01:10:40,160 --> 01:10:42,540
Y uno tiene que estar acostumbrado a que las cosas no salgan.

671
01:10:42,840 --> 01:10:45,420
Es como de los niños cuando están aprendiendo a caminar,

672
01:10:45,600 --> 01:10:48,720
que se tambalean, se caen, ni siquiera pueden natear,

673
01:10:48,820 --> 01:10:49,600
se pueden dar vuelta.

674
01:10:51,840 --> 01:10:54,400
Y así estamos cuando aprendemos matemática.

675
01:10:54,660 --> 01:10:56,460
Yo lo tengo completamente interiorizado.

676
01:10:56,580 --> 01:10:58,980
cada vez que aprendo algo nuevo, no entiendo nada.

677
01:10:59,440 --> 01:11:04,720
No entiendo nada todo con, no sé nada, pero me relajo y pienso y lo

678
01:11:05,100 --> 01:11:07,020
mire un día, después lo vuelvo a mirar otro día.

679
01:11:07,100 --> 01:11:10,460
Por ejemplo, en física típicamente los ejercicios no salen.

680
01:11:11,120 --> 01:11:13,520
Uno se puede hacerlo y para ésta tres días con un ejercicio.

681
01:11:14,200 --> 01:11:18,200
Claro, la carga horaria a veces de esas carreras son muy pesadas.

682
01:11:19,280 --> 01:11:20,000
Pero bueno, es así.

683
01:11:20,740 --> 01:11:23,340
Entonces acá mi recomendación para este curso es que,

684
01:11:23,580 --> 01:11:31,140
Aparte de lo que veamos en la clase, ustedes en su casa intenten hacer ejercicios, si se

685
01:11:31,220 --> 01:11:35,580
quedan completamente travados, me consulten a mí, así vemos cómo lo podemos resolver,

686
01:11:36,540 --> 01:11:41,720
porque a veces si no entienden una cosa pueden entender otra, si no entienden un libro, pues

687
01:11:41,820 --> 01:11:43,360
es más fácil leer otro libro y así.

688
01:11:44,600 --> 01:11:50,840
Así que bueno, es importante que haya feedback entre nosotros que se consulten también entre

689
01:11:50,840 --> 01:11:52,460
ustedes si se pueden pegar a

690
01:11:52,560 --> 01:11:54,700
algunos que saben más mejor y

691
01:11:55,080 --> 01:11:57,440
también que intenten hacer por sus

692
01:11:57,560 --> 01:11:59,820
propios medios que los hagan ustedes en

693
01:11:59,840 --> 01:12:01,340
sus casas de nuevo en ese ejercicio.

694
01:12:02,560 --> 01:12:08,560
Entonces bueno, bien, me parece que por

695
01:12:08,660 --> 01:12:12,500
esto bueno hacer un... porque ya pasó

696
01:12:12,600 --> 01:12:13,340
una hora y media, ¿no?

697
01:12:13,700 --> 01:12:17,960
Sí, hagamos un intervalo de 15 minutos, ¿te parece?

698
01:12:19,600 --> 01:12:20,880
Perfecto, pero fue...

699
01:12:21,160 --> 01:12:21,380
Sí.

700
01:12:22,140 --> 01:12:22,560
Excelente.

701
01:12:23,240 --> 01:12:25,200
Entonces nos vemos sí, 45, ok?

702
01:12:26,740 --> 01:12:28,800
Ponte para fumatear un poco de interludio.

703
01:12:30,440 --> 01:12:31,420
Ah, claro.

704
01:12:33,040 --> 01:12:33,360
Ah.

705
01:12:34,220 --> 01:12:35,380
Claro, y sí.

706
01:12:37,560 --> 01:12:38,780
Sí, sí, sí, claro, bueno.

707
01:12:39,980 --> 01:12:43,180
Bueno, si se quedan al intervalo de radio, ¿no?

708
01:12:43,420 --> 01:12:44,960
¿Por qué la anotación de vector así?

709
01:12:45,220 --> 01:12:47,440
Bueno, el drive.

710
01:12:48,020 --> 01:12:49,320
Sí, está disponible.

711
01:12:51,180 --> 01:12:52,200
¿Por qué no me...

712
01:12:52,300 --> 01:12:54,760
A ver, estoy mandando el enlace de drive.

713
01:12:55,020 --> 01:12:56,500
Voy respondiendo a poco.

714
01:12:58,500 --> 01:12:59,820
A medida que surgen las preguntas.

715
01:13:00,460 --> 01:13:01,100
World Drive.

716
01:13:05,780 --> 01:13:07,740
Bien, ¿por qué la anotación de vectores?

717
01:13:08,240 --> 01:13:10,120
Yo voy abriendo el libro de Nielsen y Schwamm.

718
01:13:14,900 --> 01:13:22,720
La notación esa que estoy usando se llama notación de KETS y es más en general la notación de

719
01:13:22,740 --> 01:13:30,400
bracket y tiene que ver con que usar esa notación después simplifica hacer algunos cálculos,

720
01:13:32,240 --> 01:13:34,480
hacer algunos cálculos que son importantes,

721
01:13:37,080 --> 01:13:43,020
pero bueno es una notación que se usa en física cuántica y en teoría de información cuántica

722
01:13:43,020 --> 01:13:49,080
también como el padre nuestro como y yo sé las estoy metiendo de una para que

723
01:13:52,780 --> 01:13:55,720
para que se vayan acostumbrando porque la vamos a usar en el curso

724
01:14:05,760 --> 01:14:06,240
no

725
01:14:11,800 --> 01:14:16,360
Bien, ya lo voy dejando de otra.

726
01:14:16,580 --> 01:14:18,780
Después, ¿por qué números complejos en cuántica?

727
01:14:20,000 --> 01:14:21,420
Bien, es una historia muy larga.

728
01:14:22,460 --> 01:14:26,480
La cuestión es que cuando se empezaban a estudiar los

729
01:14:26,680 --> 01:14:30,380
fenómenos cuánticos, lo primero que se vio era eso, ¿no?

730
01:14:33,140 --> 01:14:35,540
Sí, sí, implementála, implementála, sé mi caso.

731
01:14:36,640 --> 01:14:39,060
Yo estoy haciendo con una historia muy larga corta,

732
01:14:39,140 --> 01:14:42,920
pero vos créeme sigamente y usá esto de esta notación.

733
01:14:43,900 --> 01:14:44,560
Grate tranquilo.

734
01:14:45,260 --> 01:14:48,040
Después vas a ver que en algunos cálculos te vas a simplificar la vida.

735
01:14:49,580 --> 01:14:53,980
Lo que se descubrió es que lo importante era describir las probabilidades.

736
01:14:54,220 --> 01:14:58,240
Entonces describían, por ejemplo, probabilidades de transición

737
01:14:58,490 --> 01:15:00,280
entre niveles energéticos del átomo.

738
01:15:00,680 --> 01:15:07,020
Entonces vos tenías un nivel energético, otro y otro, y vos había...

739
01:15:07,380 --> 01:15:11,420
el átomo podría transicionar de un estado de un objeto a otro.

740
01:15:12,380 --> 01:15:17,240
Y lo que vieron es que la forma más adecuada de representar eso era por números complejos.

741
01:15:20,000 --> 01:15:21,280
Ahora, ¿qué pasa?

742
01:15:22,300 --> 01:15:28,140
Después, eso fue al principio de la cuántica, en el año 2024, 25, 26,

743
01:15:28,540 --> 01:15:32,660
después vinieron bono y manipulos, bueno, en realidad no,

744
01:15:32,660 --> 01:15:37,960
Hilbert y discípulos, fíjense que interesante, el gran matemático David Hilbert tenía como

745
01:15:38,040 --> 01:15:43,760
discípulo matemático von Neumann, también tenía Norgen, no sé si Norgen me era grosso o no,

746
01:15:45,000 --> 01:15:51,780
pero von Neumann era muy grosso, tan grosso o más grosso que Hilbert y el tipo les encomendó

747
01:15:52,460 --> 01:15:57,380
axiomatizar la teoría cuántica y bueno la forma que encontraron fue la despacio de Hilbert,

748
01:15:58,159 --> 01:16:05,060
pero la noción de espacio de Hilbert era anterior a la física cuántica, eso ya lo habían descubierto

749
01:16:05,260 --> 01:16:11,700
para otra cosa, para estudiar espacios de funciones creo, y encontraron que la forma más natural de

750
01:16:11,800 --> 01:16:17,860
representar las cuentas que hacían los físicos eran en el espacio de Hilbert. Entonces de ahí viene

751
01:16:18,360 --> 01:16:27,400
esta costumbre de utilizar espacios vectoriales complejos que cumplen con una cierta condición

752
01:16:27,400 --> 01:16:32,500
o por lógica que sería la completitud y que se conocen como espacios de Hilbert.

753
01:16:34,920 --> 01:16:41,540
Si, no respondí tu pregunta de por qué no me lo complejo porque en realidad no se sabe.

754
01:16:42,040 --> 01:16:50,960
Hay, vos podés hacer, claro, si, los quetzelobras. Hay, vos podés hacer una cuántica real que es

755
01:16:50,960 --> 01:16:58,860
bastante descriptiva y si te fijas en la literatura vas a ver que hay gente que intenta comparar

756
01:16:58,880 --> 01:17:03,780
la cuántica con números reales con la cuántica con números complejos, depende como la edad,

757
01:17:03,820 --> 01:17:08,440
te quedan que no son equivalentes y la que se tiene que usar es la que tiene números

758
01:17:08,500 --> 01:17:14,500
complejos. Por ahí vos podrías decir que empíricamente tenés que usar la que tiene

759
01:17:14,560 --> 01:17:19,360
números complejos, pero no es una buena respuesta, es porque es una respuesta muy para salir

760
01:17:19,360 --> 01:17:25,340
del paso, bueno se sabe por qué exactamente. Y así como tienes una una cuántica con números

761
01:17:25,600 --> 01:17:30,720
reales también y con números complejos, tienes una cuántica con números cuaterniónicos,

762
01:17:31,440 --> 01:17:35,800
porque los matemáticos podrán saber que tal, así como están los complejos están

763
01:17:35,800 --> 01:17:48,780
los cuaterniones. Entonces, entonces eso. Pero la posta es la que tiene números complejos,

764
01:17:49,040 --> 01:17:54,500
la que vamos a usar, lo oficial. Pero sépalo, hay muchas formulaciones de la cuántica,

765
01:17:55,600 --> 01:18:02,400
son equivalentes entre sí y son muy distintas. La que es más popular es esta que estoy dando

766
01:18:02,480 --> 01:18:07,020
yo ahora, sobre todo en teoría de información cuántica. Sí, von Neumann, claro, claro,

767
01:18:07,780 --> 01:18:13,960
sí, sí, exacto. No, no, no, von Neumann era, es un tipo muy, muy pesado, muy pesado, hizo

768
01:18:13,960 --> 01:18:19,420
con traducciones muy grandes en la matemática, pero también en la física teórica. De hecho,

769
01:18:20,560 --> 01:18:26,160
el libro de von Neumann es el que le da la forma final al formalismo cuántico. Al final del día,

770
01:18:26,360 --> 01:18:32,420
lo que yo voy a explicar acá es el libro de von Neumann, pero rebajado a un nivel muy elemental.

771
01:18:32,440 --> 01:18:54,840
en el fondo. Sí, yo igual, sí, por ahí la mejor forma de responder esa pregunta es con un

772
01:18:57,680 --> 01:19:05,980
problema abierto, ¿no? Decirte que en realidad hay un área de investigación de los fundamentos de la

773
01:19:06,020 --> 01:19:12,140
física cuántica que se encarga de intentar determinar por qué el formalismo cuántico es como ves.

774
01:19:13,820 --> 01:19:19,180
Y en eso se da mucha energía para entender por qué las cosas son así. Yo de hecho he trabajado en eso

775
01:19:19,240 --> 01:19:27,840
mucho, pero la respuesta es que no se sabe en realidad, esa es la realidad. Bueno, iba a la

776
01:19:27,850 --> 01:19:36,160
otra pregunta que era clase 1, bien. Vamos a compartir el link por el chat así.

777
01:19:43,440 --> 01:19:47,960
Sí, por ejemplo, hay muchas formas de hacerlo. Ahí está el Google Drive,

778
01:19:50,900 --> 01:19:56,700
porque Jorge, vos me habías pedido el link de Drive. Ahí te lo compartí. Fijate si

779
01:19:57,640 --> 01:20:02,020
puedes acceder y me debería llegar a mí tu solicitud.

780
01:20:08,160 --> 01:20:14,260
Bien, perfecto. Fijate si puedes entrar. Camilo, por favor, adelante Camilo.

781
01:20:15,560 --> 01:20:24,580
Ehh, Fede, bueno, ahora que están hablando los números complejos, yo quería saber si en algún momento del curso vamos a hablar, bueno,

782
01:20:24,580 --> 01:20:33,120
a tochar de una manera vaga la ecuación de Schrodinger, digamos, para hablar de probabilidad o cuestiones así.

783
01:20:34,320 --> 01:20:37,960
Sí, exacto. De una manera vaga, vamos a darme Cozende Schrodinger.

784
01:20:38,720 --> 01:20:45,580
Pero de una manera muy vaga, porque te lo comento acá, voy a volar sobre eso, pero te lo comento ahora porque...

785
01:20:50,140 --> 01:20:59,360
Porque lo que te da la Cozende Schrodinger es cómo evoluciona el estado.

786
01:21:00,960 --> 01:21:10,760
Vos tenés vas a tener un estado a tiempo cero y la ecuación de Schrodinger lo que te va a decir es cómo evoluciona la función del tiempo.

787
01:21:12,860 --> 01:21:19,500
Y en lo que vamos a ver nosotros en el fondo de ecuación de Schrodinger es equivalente a esto.

788
01:21:21,560 --> 01:21:27,640
Y acá es el número complejo, h va a ser el hamiltoniano del sistema, te va a hacer un operador lineal.

789
01:21:30,900 --> 01:21:38,400
Entonces, esto es e exponencial de e a la menos y sobre h barra de esta matriz, la exponencial de una matriz

790
01:21:40,320 --> 01:21:45,600
por el tiempo, por psíde 0, esto es igual a psíde t, ok?

791
01:21:46,440 --> 01:21:49,520
Esto es la ecuación de Schrodinger escrita de una forma muy conveniente.

792
01:21:51,800 --> 01:21:56,640
Si vos derivas esto, si haces tipo la diferencia, te queda la ecuación de Schrodinger, ok?

793
01:21:56,960 --> 01:22:03,100
acá el jamitoniano tiene que ser independiente del tiempo y así va a ser nuestro curso. Bien.

794
01:22:03,600 --> 01:22:08,880
O sea que... ¿no vas siguiendo? Sí, o sea que básicamente ahí tú estás

795
01:22:08,960 --> 01:22:15,120
expresándolo de forma matricial, la ecuación de Rodin. Claro, porque sí, sí, sí, porque

796
01:22:15,280 --> 01:22:23,560
mira, porque mira, nosotros, mira, el modelo más general de cuántica es o cuántica de

797
01:22:23,560 --> 01:22:31,220
la partícula puntual es sl2, que sería el conjunto de las f tales que integral, vos

798
01:22:31,220 --> 01:22:44,800
sos matemático, no fue el cuadrado de x menor que infinito, ok? Es decir, las f que van de

799
01:22:46,040 --> 01:22:51,820
de R3 suponente a los complejos que son cuadro integrables, ok?

800
01:22:55,520 --> 01:23:06,620
Eso es L2, pero en información cuántica y en computación cuántica no es siempre así,

801
01:23:06,760 --> 01:23:13,520
pero el uso más común es usar sistemas de dimensión finita. Entonces este es el espacio

802
01:23:13,520 --> 01:23:20,580
del Hilbert, L2, que este es isomorfo a, si querés, ya vemos, L2 que sería L2, sería

803
01:23:21,980 --> 01:23:30,780
la sucesiones CN tales que suma de módulo del CN al cuadrado, al infinito es menor que

804
01:23:30,840 --> 01:23:37,920
infinito, ¿eh? Las sucesiones que convergen en suma módulo cuadrado, ¿ok? Bueno, como

805
01:23:37,920 --> 01:23:43,740
bien sabes, se le dos estos espacios son isomorfos y son el espacio de Hilbert, ok?

806
01:23:47,120 --> 01:23:53,840
bien, pero nosotros en este curso no vamos a ver eso, no vamos a ver eso porque es un quilombo,

807
01:23:53,940 --> 01:23:59,140
pues ya es un quilombo explicar al general y vamos, la gente no tiene vacas para dar todo esto,

808
01:23:59,360 --> 01:24:02,520
esto por ahí en física se ve pero

809
01:24:06,380 --> 01:24:09,580
pero si vamos a concentrar el sistema que tiene

810
01:24:09,600 --> 01:24:11,700
dimensión finita por ejemplo un sistema

811
01:24:11,800 --> 01:24:16,540
spin medio o suponerte más fácil un átomo

812
01:24:18,280 --> 01:24:20,480
en el cual usted concentra en dos niveles de energía

813
01:24:22,400 --> 01:24:25,360
el nivel 0 y el nivel 1

814
01:24:25,360 --> 01:24:30,100
Entonces la idea es que esto lo vas a describir por C2. Entendás?

815
01:24:31,659 --> 01:24:33,860
Ok, Fede usar básicamente...

816
01:24:33,880 --> 01:24:44,600
Fede usar L2, esta es cuántica. Si vos quisieras describir cómo un electrón se mueve libremente en el vacío o si quieres

817
01:24:45,360 --> 01:24:52,140
todos los niveles energéticos del átomo, tenés que usar el E2, pero si te concentras solo en dos

818
01:24:52,220 --> 01:25:01,820
niveles usas el E2, y si te concentras en tres niveles usas el E3, ¿entendés?

819
01:25:02,400 --> 01:25:08,820
Sí, sí, sí. Y así vas a usar CN y lo que vamos a usar en información cuántica es cuando tengas una

820
01:25:08,920 --> 01:25:14,960
computadora cuántica que va a ser un átomo, otro átomo con dos niveles, otro átomo con dos niveles,

821
01:25:14,960 --> 01:25:23,540
Entonces vas a tener C2, C2 y C2 y el espacio total va a ser C2 por C2 por C2 que va a ser C8, ¿entiendes?

822
01:25:24,440 --> 01:25:31,240
Claro, claro, entiendo. O sea que básicamente nosotros vamos a trabajar con la dimensión finita, porque estamos ahí.

823
01:25:31,240 --> 01:25:32,760
Exacto. Ok, ok.

824
01:25:33,699 --> 01:25:40,960
Exactamente. Por una cuestión de que la mayoría de, digamos, para entender la teoría de la computación cuántica

825
01:25:40,960 --> 01:25:43,540
y la mayoría de los protocolos de información cuántica,

826
01:25:43,700 --> 01:25:47,300
no todos, pero la mayoría, te alcanza con dimensión finita.

827
01:25:48,800 --> 01:25:49,320
Vale, vale.

828
01:25:49,480 --> 01:25:53,420
Bueno, Fede, mira, yo el semestre pasado vi un curso de

829
01:25:53,440 --> 01:25:58,380
algebra lineal que básicamente era pura dimensión finita y

830
01:25:58,420 --> 01:26:02,000
tocar el tema de espacios producto interno.

831
01:26:02,760 --> 01:26:05,840
O sea, básicamente el tratamiento que es que se le está dando y

832
01:26:05,940 --> 01:26:08,520
yo tenía esa duda, ¿será que en el curso vamos a trabajar

833
01:26:08,520 --> 01:26:11,700
con dimensión finita o con dimensión infinita en el espacio pictorial.

834
01:26:12,460 --> 01:26:13,080
Pero, ¿ya tú quieres?

835
01:26:13,870 --> 01:26:13,980
Claro, claro, claro.

836
01:26:15,620 --> 01:26:16,460
Claro, entonces sí.

837
01:26:19,000 --> 01:26:26,460
Sí, porque la cuántica en el final de 2, el fondo ya es análisis funcional, ya no es más álgebra lineal, ¿entendés?

838
01:26:27,040 --> 01:26:30,400
Pugote, tenés que meter con operadores autodjuntos, ¿viste?

839
01:26:33,380 --> 01:26:39,140
que yo por ejemplo fíjate que un átomo puede dar niveles de energía discretos pero después

840
01:26:40,340 --> 01:26:47,520
los estados ligados son discretos pero los estados libres son continuos entonces el espectro

841
01:26:49,190 --> 01:26:55,360
lo vas a representar por un operador autodjunto que va a tener un espectro que parte es discreta y

842
01:26:55,360 --> 01:26:56,580
partes continuos, ¿entendés?

843
01:26:58,450 --> 01:27:00,800
Y entonces ahí te viene como anillo al nivel análisis

844
01:27:00,920 --> 01:27:03,060
funcional, pero ya eso tiene un nivel de complejidad

845
01:27:03,080 --> 01:27:06,640
matemática que excede muchísimo este curso.

846
01:27:09,780 --> 01:27:16,920
Y dicho sea de paso, fue un gran contributor,

847
01:27:17,200 --> 01:27:21,180
sería un gran contribuyente a la teoría del análisis

848
01:27:21,240 --> 01:27:24,680
funcional y en particular desarrolló la teoría de

849
01:27:24,680 --> 01:27:27,120
anillos de operadores y la lógica cuántica.

850
01:27:29,960 --> 01:27:34,840
Y a partir de eso se desarrollan las estrellas algebras y que se llaman.

851
01:27:37,860 --> 01:27:41,680
Pero bueno, acá estamos así. Bien, termina el diálogo. Genial.

852
01:27:44,120 --> 01:27:48,620
Seguimos ahí, compartir la... ah, ahí está.

853
01:27:50,460 --> 01:27:53,280
Vamos a resolverlo del like porque... ah, acá estamos.

854
01:27:54,680 --> 01:27:56,100
acá estaban todos

855
01:27:58,580 --> 01:28:00,520
vamos a compartir así ya

856
01:28:13,320 --> 01:28:16,540
bueno entonces ahora vamos a ver otras

857
01:28:18,340 --> 01:28:22,200
propiedades que son cruciales

858
01:28:23,460 --> 01:28:26,020
de los espacios vectoriales

859
01:28:29,980 --> 01:28:32,080
y igual miren la primera clase era muy

860
01:28:32,180 --> 01:28:35,380
como pantallazo general yo creo que ya la clase

861
01:28:36,760 --> 01:28:39,340
propiamente posta el curso sexta que es

862
01:28:39,340 --> 01:28:40,180
por el más aburrida

863
01:28:43,280 --> 01:28:47,200
bien, ahí está, ahí es compartido

864
01:28:48,200 --> 01:28:49,780
Bueno, vuelvo esto.

865
01:28:52,640 --> 01:29:02,260
Ah, bien, después se los mando por mensajes general, pero tienen que leer esto, tienen

866
01:29:02,260 --> 01:29:11,700
que leer entre esta clase y la que viene tienen que intentar leer todo el capítulo 1 del

867
01:29:11,720 --> 01:29:12,480
el senichón

868
01:29:16,420 --> 01:29:21,400
y empezar a leer el capítulo 2 la parte algerenial acá

869
01:29:24,540 --> 01:29:25,720
tienen que leer 2 1

870
01:29:30,420 --> 01:29:35,540
2 1 1 y con lo que vamos a ver hoy pueden leer hasta acá

871
01:29:36,680 --> 01:29:39,220
este lo si quieren lo pueden empezar a leer pero

872
01:29:41,400 --> 01:29:46,400
pero no vamos a ver hoy eso bien y ven que ya empieza a tener ejercicios

873
01:29:46,600 --> 01:29:51,620
mi recomendación es que vayan haciendo meticulosamente estos ejercicios y lo

874
01:29:51,660 --> 01:29:59,060
hablé con la gente de una UR que hacer con el inglés lo que me decían es bueno

875
01:29:59,600 --> 01:30:03,321
yo aparte les voy a dar ejercicios así que los que no entienden nada en inglés

876
01:30:03,320 --> 01:30:08,420
también van a tener la oportunidad de hacer ejercicios, pero que tomen luego como un desafío de la

877
01:30:08,460 --> 01:30:13,440
materia, como un aprendizaje. ¿Por qué? Porque me estuve fijando y no encuentro la traducción de

878
01:30:13,460 --> 01:30:23,300
este libro al Castellano. Y eso es algo que para estas artes extravagantes, todo lo que sea tecnológico,

879
01:30:23,700 --> 01:30:28,921
para encontrar tecnológico, científico, a un nivel avanzado, va a encontrar que gran parte de la

880
01:30:28,920 --> 01:30:35,200
literatura no está en español. Y entonces ustedes como profesionales no se pueden limitar

881
01:30:35,920 --> 01:30:41,320
lamentablemente. Argentina es un país que no es subdesarrollado, está en vida

882
01:30:41,400 --> 01:30:46,260
desarrollarse, bueno es un poco ideológica esa caracterización pero no es como

883
01:30:46,360 --> 01:30:51,720
alemania o como como inglaterra, yo qué sé decir. Tenemos muchas falencias en

884
01:30:51,760 --> 01:31:03,100
particular tenemos lamentablemente una dependencia tecnológica. Entonces nosotros para poder seguir

885
01:31:03,320 --> 01:31:10,220
la carrera tenemos que sí o sí tratar de adaptarnos a este mundo que está cambiante. Entonces una cosa

886
01:31:10,220 --> 01:31:19,601
que les enseña la facultad es aprender inglés porque después para manejarse a nivel laboral lo van a

887
01:31:19,600 --> 01:31:26,180
necesitas. Entonces, ah, el esfuerzo hoy con chat GPT pueden hacer así, copy, paste,

888
01:31:26,420 --> 01:31:31,420
y lo van traduciendo línea por línea. Y estos libros se leen así, no se leen como

889
01:31:31,420 --> 01:31:36,180
si fuera el diario o como una revistita. Tienen que leerlo de línea por línea y entender

890
01:31:36,300 --> 01:31:42,660
todo matemáticamente. Entonces, primero intentan entender esto, una vez que terminan de entender

891
01:31:42,780 --> 01:31:49,580
esto, después siguen. Y es muy importante que van eso y que se acostumbran a leer

892
01:31:50,000 --> 01:31:58,080
son libros científicos, no son libros de literatura. Tienes que leer meticulosamente y volver una y otra

893
01:31:58,240 --> 01:32:03,700
vez. Si hay algo que no lo entienden, bueno, lo dejan de leer hoy, para de leer y lo siguen leyendo

894
01:32:03,780 --> 01:32:10,700
mañana lo mismo, una y otra vez, como los bebés cuando le ponen debo y lo ven 500 veces a la misma

895
01:32:10,800 --> 01:32:16,420
película o en la casa se lo mismo. Y siempre estamos así, yo sigo así, aprendo así, cuando tengo

896
01:32:16,420 --> 01:32:22,200
aprender algo nuevo, no hay otro camino. Bien, sigo.

897
01:32:24,780 --> 01:32:26,320
Sigo con la clase.

898
01:32:28,719 --> 01:32:30,080
¿Me impuso algo ahí?

899
01:32:34,440 --> 01:32:34,540
No.

900
01:32:36,500 --> 01:32:36,680
Bien.

901
01:32:38,280 --> 01:32:44,900
Bueno, vimos entonces el concepto de espacio vectorial

902
01:32:44,900 --> 01:32:50,140
complejo, que es lo mismo que el concepto de espacio vectorial real, nada más que ahora

903
01:32:51,520 --> 01:32:58,100
las conrederadas o los componentes de los vectores son números complejos y cuando multiplican

904
01:32:58,560 --> 01:33:01,300
a un vector también lo pueden multiplicar por un número complejo.

905
01:33:03,140 --> 01:33:08,260
Ah, y una cosa que me olvide decirles antes que es súper importante, es que en el curso

906
01:33:08,260 --> 01:33:10,060
también vamos a ver matrices.

907
01:33:11,560 --> 01:33:16,380
Y yo les decía antes a alguien que no conoce esto,

908
01:33:16,400 --> 01:33:18,840
poder decir, bueno, ¿para qué te gastas, Federico,

909
01:33:19,160 --> 01:33:21,680
en dar los acciones a un espacio vectorial?

910
01:33:21,760 --> 01:33:22,180
¿Por qué no?

911
01:33:22,360 --> 01:33:23,140
Directamente.

912
01:33:23,840 --> 01:33:27,340
¿Por qué directamente no me das los ejemplos de espacios

913
01:33:27,360 --> 01:33:27,920
vectoriales?

914
01:33:27,980 --> 01:33:31,600
Bueno, está bueno tener esta noción abstracta de espacios

915
01:33:31,680 --> 01:33:36,900
vectorial porque es un concepto que subsume a entes

916
01:33:36,900 --> 01:33:43,000
bastante distintos entre sí. Ya vimos que, por ahora, vimos varios ejemplos de

917
01:33:43,020 --> 01:33:51,920
espacio vectoriales, vimos Rn, estos eran los que eran columnas de números reales,

918
01:33:52,420 --> 01:34:00,720
vimos CN que eran columnas de n números complejos, 1, 2, 3, 4, las que sean y

919
01:34:00,720 --> 01:34:06,560
y después la otra cosa que hay es Rn por m, que serían las matrices por ejemplo.

920
01:34:08,940 --> 01:34:17,080
Nosotros describimos a los vectores como columnas de números reales o complejos.

921
01:34:18,780 --> 01:34:20,880
¿Y qué pasa si ahora les doy algo así?

922
01:34:21,720 --> 01:34:27,160
A es igual a 1, 2, 3, 4, 5, 6, 7, 8, 9.

923
01:34:28,720 --> 01:34:40,160
esto, a matrix que decimos que pertenece a, tiene 3 filas y 3 columnas, 3 por 3

924
01:34:41,010 --> 01:34:56,040
y así, y también podrían tener una matrix que si yo ve que sea -1, 2, 5, 1, 1, 1 y esta pertenece a la 2 por 3

925
01:34:56,040 --> 01:35:02,700
Y así siguiendo, en general va a tener r a la n por m, es decir,

926
01:35:03,760 --> 01:35:10,000
matrices que serían arreglos cuadrados de números reales o complejos de n filas y m columnas.

927
01:35:10,450 --> 01:35:13,060
Y también van a tener c a la n por n.

928
01:35:15,280 --> 01:35:18,100
Estos también son ejemplos de espacios vectoriales.

929
01:35:19,740 --> 01:35:24,580
Esto es importante entenderlo. Por ejemplo, abremos una matriz.

930
01:35:25,900 --> 01:35:34,280
Esta la vamos a hablar del curso, no? Sigma x sería 0, 1, 1, 0. Sigma y sería 0 menos

931
01:35:34,580 --> 01:35:47,700
y y 0. Sigma z igual a 1, 0, 0 menos 1. Estas son matrices, matrices de 2 por 2. Y como

932
01:35:47,720 --> 01:35:57,600
esta por ejemplo pertenece a complejos, 2x2, son dos filas y dos columnas. Un vector de la

933
01:35:57,640 --> 01:36:12,520
forma b, del tipo b igual a alpha1, alphan, se puede pensar con una matriz de mx1, o nx1.

934
01:36:18,800 --> 01:36:28,140
R a la n por 1, ¿sí? Son n filas y una columna. O los bra que vamos a ver, estos son los kits,

935
01:36:28,470 --> 01:36:37,560
los bra que vamos a ver después, van a ser vectores filas. Esta pertenece a R a la una fila por n

936
01:36:37,560 --> 01:36:45,360
columnos. Entonces las matrices definidas de forma tosca van a ser para nosotros arreglos

937
01:36:45,440 --> 01:36:51,280
cuadrados de números de distintos tamaños. Lo importante es que uno puede sumar matrices,

938
01:36:51,320 --> 01:37:01,040
por ejemplo si sumo sigma x más sigma y me queda 0 1 1 a 0 y más 0 menos y y 0. Y cómo se suman?

939
01:37:01,040 --> 01:37:06,300
Bueno en forma análoga a la que se suman los vectores. Tengo que sumar coordenada, coordenada,

940
01:37:06,300 --> 01:37:12,120
0 más 0, 1 más menos y, perdón,

941
01:37:16,020 --> 01:37:21,400
1 más y y después 0 más 0, y esta me queda esa matriz.

942
01:37:23,670 --> 01:37:29,320
Y también se multiplican por escalares, ya sé que yo 2 por sigma y les queda 2 por

943
01:37:29,320 --> 01:37:37,160
por 0 menos i y 0 y queda 0 menos 2i, 2i y 0.

944
01:37:38,719 --> 01:37:45,200
Entonces, las matrices también forman espacios vectoriales,

945
01:37:45,740 --> 01:37:48,680
porque la suma y multiplicación por escala de las matrices

946
01:37:51,640 --> 01:37:56,140
tienen la cumple con los axiomas de espacios vectoriales.

947
01:37:56,200 --> 01:38:06,300
Entonces le dejo como ejercicio verificar que, por ejemplo, las matrices de 2 por 2 complejas son un espacio vectorial.

948
01:38:10,060 --> 01:38:12,340
Es un espacio vectorial.

949
01:38:14,840 --> 01:38:21,080
Y entonces, todas las propiedades generales de los espacios vectoriales se aplican a matrices.

950
01:38:22,140 --> 01:38:25,880
Hay cosas que valen para vectores y que no valen para matrices, y dice Barça.

951
01:38:26,000 --> 01:38:31,300
En realidad, perdón, los hectares son el caso particular de Matrises, se los acabo de decir, pero

952
01:38:33,000 --> 01:38:41,820
la gracia es que hay, si uno abstrae el concepto de espacio vectorial, se va a encontrar con que

953
01:38:41,880 --> 01:38:48,540
existen muchos entes matemáticos que cumplen con la noción de espacio vectorial, pero que son

954
01:38:48,560 --> 01:38:55,900
muy diferentes entre sí. Por ejemplo, los polinomios forman un espacio vectorial para

955
01:38:55,980 --> 01:39:00,600
que se den la función, uno puede tener un espacio vectorial de funciones y de ahí

956
01:39:01,130 --> 01:39:06,300
que uno estudiando las propiedades algebraicas de los espacios vectoriales obtiene una herramienta

957
01:39:06,340 --> 01:39:10,840
muy poderosa para hacer desarrollos en matemática y en física. Entonces, por eso es importante

958
01:39:12,560 --> 01:39:18,880
lo vamos a ver ahora con el concepto de base, ahora se lo voy a ver, pero entonces hoy definimos

959
01:39:19,040 --> 01:39:29,040
espacio vectorial y tenemos muchos ejemplos del espacio vectorial, rn, cn y después r al n por m

960
01:39:30,740 --> 01:39:37,940
y c a la n por m y a r, n y a cm la pon ver como casos particulares de cada uno de estos donde

961
01:39:41,500 --> 01:39:42,580
m es igual a 1.

962
01:39:45,900 --> 01:39:52,500
Es bueno, espacio a esperar. Y ahora vamos a ver algo que es crucial y que se va a ver a lo largo de

963
01:39:52,600 --> 01:39:57,520
todo el curso o va a estar implicitamente en las cuentitas de todo el curso que es

964
01:39:59,540 --> 01:40:01,280
el concepto de combinación lineal.

965
01:40:03,760 --> 01:40:05,220
Primero le voy a motivar,

966
01:40:07,900 --> 01:40:11,340
lo voy a motivar con un dibujo.

967
01:40:15,360 --> 01:40:16,920
Supongo que estamos en R3,

968
01:40:20,340 --> 01:40:24,700
son vectores con tres coordenadas, X, Y y Z.

969
01:40:25,640 --> 01:40:34,860
consideramos el plano X y y consideramos un vector que no está en el plano X y este B está

970
01:40:35,120 --> 01:40:40,860
afuera del plano X y y W si está en el plano X y si

971
01:40:44,719 --> 01:40:49,320
bien W si uno considera por ejemplo el vector

972
01:40:52,920 --> 01:41:05,100
llamémosle b0 igual a 1 0 0, es el que tiene 1 1 en x y 0 y 0 en y y b1 en el 0 1 0.

973
01:41:07,060 --> 01:41:14,540
Entonces, W está dentro del plano, está contenido en el plano, es coplanar con b0 y b1.

974
01:41:17,500 --> 01:41:30,940
Por lo tanto uno puede encontrar multiplicar a b0 y a b1 por escalares y sumarlos y escribir a w en función de b0 y b1.

975
01:41:31,820 --> 01:41:37,720
Por ejemplo, supongo que tenemos w igual a 2, 3 y 0.

976
01:41:39,140 --> 01:41:39,500
Entonces

977
01:41:46,000 --> 01:41:58,360
W es 2, 3, 0. W se puede escribir como 2 por 1, 0, 0 más 3 por 0, 1, 0 más 0 por 0, 0, 1.

978
01:41:59,580 --> 01:42:01,440
Este último no lo pongo porque vale 0.

979
01:42:03,180 --> 01:42:10,160
Entonces esto prueba que W es 2 por B0 más 3 por B1.

980
01:42:14,400 --> 01:42:18,300
Y esto quiere decir que W está incluido en el plano

981
01:42:20,350 --> 01:42:28,640
que genera B0 y B1. Ven que loco Juan, es loco que me cuesta explicarlo sin usar los conceptos que

982
01:42:28,640 --> 01:42:36,660
tengo que explicar, está tan grabado en la mente que van. Pero bueno, la gracia es que

983
01:42:37,920 --> 01:42:46,520
si uno hace múltiplos por escalares y sumas de B0 y B1, va a terminar generando todo el

984
01:42:46,620 --> 01:42:53,880
plano de XI. Entonces, decimos que W es combinación lineal de B0 y B1. ¿Por qué? Porque se puede

985
01:42:53,880 --> 01:43:00,560
escribir así como algo por 0 más algo por 1 y decimos que el b que estaba fuera del plano

986
01:43:01,500 --> 01:43:05,960
no es combinación lineal de ellos ¿Por qué? Porque no va a existir ningún numerito,

987
01:43:07,360 --> 01:43:11,260
ningún numerito ni combinación de sumas ni de nada tal que yo le puedo escribir como

988
01:43:11,380 --> 01:43:18,120
del plano. Entonces ese es el concepto de combinación lineal y va a estar vinculado al concepto de

989
01:43:18,120 --> 01:43:26,960
dependencia e independencia lineal, ya lo vamos a ver después. Entonces, W es combinación

990
01:43:27,100 --> 01:43:35,020
lineal, entonces ahora vamos a dar la definición abstracta, dado un espacio vectorial B, ya

991
01:43:35,020 --> 01:43:39,920
sea sobre los números reales o los complejos, y piensen que ahora B no necesariamente es

992
01:43:40,020 --> 01:43:46,740
el retrezo o el plano, sino que podrán hacer un espacio de matrices. Supongamos que

993
01:43:46,740 --> 01:43:52,140
B1 hasta Bn son vectores de B. Decimos que B, acá me comí, tendría que haber puesto,

994
01:43:54,220 --> 01:44:00,000
me faltó ponerle la notación que está mal, pero va el por lo que un vector es combinación

995
01:44:00,100 --> 01:44:06,420
lineal de B1 Bn, si existen unos números, ya sean en erro en C, dependiendo el caso de

996
01:44:06,520 --> 01:44:12,700
que B sea complejo de real, de forma tal de que B se escriba como A1 por B1 más A2 por

997
01:44:12,700 --> 01:44:18,960
2, está tratada y así siendo hasta n por bn. Esto se escribió de forma compacta así, suma,

998
01:44:19,600 --> 01:44:25,880
este sumo es sin volver al del sumatoria de i igual a 1 hasta la n de ai por bi.

999
01:44:27,739 --> 01:44:28,980
Le voy a tratar de explicar.

1000
01:44:36,900 --> 01:44:37,800
Por ejemplo,

1001
01:44:41,580 --> 01:44:49,380
si tenemos de vuelta b0 igual al 1, 0, 0 y b1 igual a 0, 1, 0, ¿no?

1002
01:44:50,420 --> 01:45:00,220
si escribo alfa por b0 más beta por b1 y esto lo llamo b, bueno b es combinación

1003
01:45:00,320 --> 01:45:07,100
lineal de b0 y b1 y del mismo modo eso lo puedo tener en cualquier espacio, si tengo

1004
01:45:07,100 --> 01:45:24,400
un espacio, el cual tengo b0, b1 hasta bn y ponemos wb igual a suma de alfa y por bi

1005
01:45:25,370 --> 01:45:34,740
con i igual a 0 hasta n menos 1, entonces wb es combinación lineal de estos, es el concepto

1006
01:45:34,740 --> 01:45:43,800
si quieren más importante de la noción de espacio vectorial, el concepto de combinación

1007
01:45:43,860 --> 01:45:50,640
lineal. Los espacios vectoriales son espacios lineales y espacios lineales quiere decir esencialmente

1008
01:45:50,860 --> 01:45:59,780
esto que pueden hacer combinaciones lineales, es la gracia del espacio vectorial. Bien, sigo.

1009
01:46:05,420 --> 01:46:13,580
Y decimos, dado un espacio vectorial sobre R o C, decimos que el conjunto, acá me comí

1010
01:46:13,620 --> 01:46:21,800
un B2, B1, B2, Bn, genera a B, si todo B del espacio vectorial se puede escribir como

1011
01:46:21,880 --> 01:46:27,220
combinación lineal del elemento de C, es decir que para cualquier vector B existen escalares

1012
01:46:27,220 --> 01:46:31,380
a una A y A, tal vez que el B se puede escribir como combinación lineal de ellos.

1013
01:46:32,980 --> 01:46:35,700
Esto es muy importante que lo entiendan con ejemplos.

1014
01:46:36,180 --> 01:46:36,820
Vamos a hacer un ejemplo.

1015
01:46:40,360 --> 01:46:41,320
Concieremos R2.

1016
01:46:44,100 --> 01:46:49,960
R2 eran todos los pares A, B, donde A y B son números reales.

1017
01:46:51,040 --> 01:46:51,200
Bien.

1018
01:46:54,020 --> 01:47:04,280
En R2 tenemos que si tomamos el conjunto por ejemplo C igual a el 1, 0 y el 0, 1

1019
01:47:07,100 --> 01:47:09,220
¿Cómo es un vector arbitrario de R2?

1020
01:47:09,440 --> 01:47:11,500
Un vector arbitrario de R2 va a ser una B.

1021
01:47:13,320 --> 01:47:18,480
Entonces yo puedo escribir a este AeB como A por 1, 0 más B por 0, 1.

1022
01:47:19,180 --> 01:47:22,980
Ven que se hacen A por 1, les queda A, A por 0 les queda 0

1023
01:47:23,700 --> 01:47:31,000
algo parecido con me y cuando suman recuperan a b. Bien, pero esto, esta ecuación de acá

1024
01:47:31,130 --> 01:47:37,260
me está diciendo que cualquier vector b, cualquier vector con a y b arbitralios, se

1025
01:47:37,400 --> 01:47:42,160
puede escribir como combinación lineal de estos dos vectorcitos de la calle, me muémosle

1026
01:47:42,260 --> 01:47:42,620
¿Qué es eso?

1027
01:47:43,960 --> 01:47:45,520
Es 0 y es 1.

1028
01:47:47,940 --> 01:47:49,960
Entonces el conjunto formado por

1029
01:47:52,159 --> 01:47:54,920
es 0 y es 1

1030
01:47:56,119 --> 01:47:56,840
genera

1031
01:47:58,180 --> 01:47:58,780
todo el redoso.

1032
01:48:06,079 --> 01:48:07,080
Y ahora

1033
01:48:12,000 --> 01:48:16,640
pensémos en esto, supongo que se prima

1034
01:48:25,800 --> 01:48:28,060
hola, hola el drive

1035
01:48:29,460 --> 01:48:34,500
si el drive solo tiene el video de la clase anterior

1036
01:48:39,260 --> 01:48:40,920
paso otra vez al vídeo

1037
01:48:43,340 --> 01:48:43,780
solo

1038
01:48:45,440 --> 01:48:48,920
si en el drive Andrea vas a ver el vídeo de la clase pasada porque solo hay una

1039
01:48:48,980 --> 01:48:53,680
clase el nuevo si se graba bien la de hoy lo subo después y se los comparto

1040
01:48:55,180 --> 01:48:55,620
este

1041
01:48:58,400 --> 01:49:00,420
así que si no debería haber ningún misterio

1042
01:49:07,420 --> 01:49:16,520
Bien, sigo. Perdón, profe, en el Drive hay solo un vídeo, nada más no tenemos los Power Point y todos esos asquivos que estamos perdiendo ustedes.

1043
01:49:18,220 --> 01:49:20,980
El Power Point está acá, espera.

1044
01:49:23,000 --> 01:49:24,580
Para mí me lo veo de vuelta y te lo muestro.

1045
01:49:30,300 --> 01:49:35,300
Al principio de todo yo puse una carpetita que dice clases y tiene el

1046
01:49:35,740 --> 01:49:39,680
Jolly Cunaúr curso 01. Esta sería el powerpoint de la primera clase.

1047
01:49:43,320 --> 01:49:51,040
Y cuando esté el de la segunda, lo subo. De llamanía, lo pasado, subo los archivos de la segunda clase.

1048
01:49:51,170 --> 01:49:55,460
Ok? Ok, y la escapacitación la tenemos en el campus también.

1049
01:49:56,260 --> 01:49:57,100
lo voy a subir mañana.

1050
01:49:58,440 --> 01:50:01,180
Entonces en el drive tenemos solo el video de las clases.

1051
01:50:02,660 --> 01:50:04,620
Claro, en el drive solo el video de las clases, si.

1052
01:50:04,840 --> 01:50:12,640
No subí la clase a la página de la materia porque por ahí es muy pesado, yo qué sé.

1053
01:50:13,040 --> 01:50:20,100
Después de acá en la bibliografía, acordate que yo les voy a dar de ejercicios a hacer cosas del libro, ok?

1054
01:50:21,080 --> 01:50:23,620
Ya sacate, podés bajar los libros, ¿entiendes?

1055
01:50:24,260 --> 01:50:28,460
claro el libro que estaba mostrando a usted ese del medio digamos

1056
01:50:29,340 --> 01:50:31,840
si el nier se le echó, yo después mando un medio y escribo bien

1057
01:50:32,420 --> 01:50:34,220
y pongo bien los capítulos para que no haya

1058
01:50:34,240 --> 01:50:37,440
no era para ubicarme porque no sabía dónde buscarlo por eso

1059
01:50:38,200 --> 01:50:42,140
claro claro, fijate ahí la página y yo después voy a ir subiendo

1060
01:50:42,360 --> 01:50:45,620
acá van cosas pero bueno por ahora tienen esto

1061
01:50:46,340 --> 01:50:47,900
y acuérdense que tienen esto

1062
01:50:48,120 --> 01:50:48,700
"Kiss it love"

1063
01:50:54,580 --> 01:50:59,400
bueno esto lo lleva acá, que acá tienen también como un cursito paralelo de computación

1064
01:50:59,520 --> 01:51:05,840
cuándica que pueden hacer y yo les recomiendo que le vayan leyendo, pero bueno pues les

1065
01:51:06,160 --> 01:51:12,260
les mando, ok?

1066
01:51:16,240 --> 01:51:19,080
bien y recuerden, ya que estamos...

1067
01:51:23,300 --> 01:51:26,660
si, el curso es este, lo mando por acá, pero está en la página de la materia

1068
01:51:29,960 --> 01:51:31,500
Y la idea es que...

1069
01:51:34,860 --> 01:51:38,960
Yo les mandé también acá también por la página de la materia.

1070
01:51:39,620 --> 01:51:39,980
Ahí está.

1071
01:51:43,380 --> 01:51:44,940
Por la página esta...

1072
01:51:49,920 --> 01:51:51,780
Yo les mandé en avisos...

1073
01:51:53,460 --> 01:51:56,640
Si se fijan en este email tiene el link a la comunidad de WhatsApp.

1074
01:51:57,620 --> 01:52:00,680
Y por ahí por la comunidad de WhatsApp podemos resolver estas cuestiones

1075
01:52:01,500 --> 01:52:03,900
las problemáticas, no? Che, no puedo acceder a esto

1076
01:52:04,280 --> 01:52:07,300
o qué ejercicio había que hacer o ese tipo de cosas

1077
01:52:07,960 --> 01:52:09,240
para hacerlo un poco más operativo

1078
01:52:10,360 --> 01:52:12,820
por ahí no respondo yo pero responde a un compañero

1079
01:52:12,860 --> 01:52:13,600
o algo así

1080
01:52:14,320 --> 01:52:16,620
así que bueno, quienes quieran se pueden sumar a la comunidad

1081
01:52:17,160 --> 01:52:18,440
pero no es oligatorio obviamente

1082
01:52:20,280 --> 01:52:23,620
bueno, estamos con las cuestiones técnicas

1083
01:52:23,760 --> 01:52:32,680
Bien, vuelvo a explicar esto de generadores. Fíjense que esto que les decía acá

1084
01:52:35,540 --> 01:52:44,540
coincide, si usar el 0 1 y el 1 0 coincide con escribir, yo tenía R2, ¿no?

1085
01:52:44,620 --> 01:52:54,420
el 1 0 es este de acá, este llamamos es 0 y el 0 1 es este de acá, el 1, ¿qué quiere decir

1086
01:52:54,660 --> 01:52:55,780
esta ecuación de acá arriba?

1087
01:53:00,160 --> 01:53:00,740
esto de acá

1088
01:53:03,060 --> 01:53:08,340
quiere decir que cualquier vez, geométricamente, se puede escribir como

1089
01:53:10,420 --> 01:53:15,840
multiplicar a es 0 por algo, multiplicar a es 1 por algo y expulsarlos, ¿sí?

1090
01:53:17,500 --> 01:53:23,560
esto es que un "b" se puede escribir como alfa por es 0, más beta por e1, ¿tabian?

1091
01:53:26,940 --> 01:53:30,960
pero por qué eso es así? bueno, porque es 0 y e1 generan todo el plano

1092
01:53:31,640 --> 01:53:35,620
¿qué pasa si ahora, en vez de usar es 0 y e1

1093
01:53:41,640 --> 01:53:47,060
uso otros vector, si? que yo en vez de usar el serie 1 podría haber usado este y este,

1094
01:53:48,220 --> 01:54:00,140
podría haber usado el que es el prima 0 igual a 1 sobre el raíz de 2, 1 sobre el raíz de 2 y el prima 1 igual a

1095
01:54:04,720 --> 01:54:07,720
menos 1 sobre raíz de 2 y 1 sobre raíz de 2.

1096
01:54:10,120 --> 01:54:14,420
Bueno, les dejo como ejercicio, y creo que está también el bien se ha hecho

1097
01:54:15,160 --> 01:54:22,840
probar que estos dos vectores también generan R2, porque cualquier vector se

1098
01:54:22,890 --> 01:54:27,420
puede escribir como combina hacia la línea de esos dos. ¿Cómo tendrían que hacer para

1099
01:54:27,500 --> 01:54:33,940
probar eso? Bueno, primero pensemos, ¿cómo es un vector arbitrario R2? Es una A,

1100
01:54:33,960 --> 01:54:43,340
donde a y b son números reales. Entonces tengo que plantear la ecuación a b igual a un número

1101
01:54:43,460 --> 01:55:00,560
alfa por 1/2, 1/2 + número beta por -1/2 y 1/2. De esta ecuación de acá obtengo que a b debería

1102
01:55:00,560 --> 01:55:08,300
ser igual, ahora sumo ¿no? Me queda alpha por 1 sobre raíz de 2 más e, menos beta por

1103
01:55:08,400 --> 01:55:14,820
1 sobre raíz de 2 y después acá me queda alpha por 1 sobre raíz de 2 más beta por

1104
01:55:14,880 --> 01:55:24,840
1 sobre raíz de 2. De acá tengo que, esto va a ser igual a esto, si a es igual a 1 sobre

1105
01:55:24,840 --> 01:55:32,360
de Rai de 2 por alfa menos beta y b es igual a 1 o Rai de 2 por alfa más beta.

1106
01:55:34,660 --> 01:55:40,600
Entonces la pregunta es si a partir de un dado a y b, ratán, son todos como un íntil,

1107
01:55:43,800 --> 01:55:50,840
yo siempre voy a poder despejar alfa y beta. Bueno, esto en el fondo es un sistema de

1108
01:55:50,840 --> 01:55:55,340
ecuaciones. TNAB escriba, ¿no?

1109
01:55:59,440 --> 01:56:03,480
Sorra y dedos, menos unos sorra y dedos.

1110
01:56:06,380 --> 01:56:10,240
Unos sorra y dedos, unos sorra y dedos. Pero tienen que despejar este sistema de ecuaciones.

1111
01:56:12,400 --> 01:56:17,300
Lo pueden hacer a mano, ¿eh? Pero bueno, se los dejo como ejercicio.

1112
01:56:19,040 --> 01:56:27,080
Espero que le salga, pero entiendo que no le va a salir a todos porque entiendo que varios de los que está acá ni siquiera entienden lo que les estoy pidiendo.

1113
01:56:27,420 --> 01:56:32,160
Entonces, bueno, piensen en esto y traten de hacerlo y la semana que viene lo resolvemos, ok?

1114
01:56:32,900 --> 01:56:40,780
Pero la idea es que cualquier vector de redos también se puede escribir como combinación lineal de zordo.

1115
01:56:40,840 --> 01:56:44,420
Entonces el conjunto C iguala 1, 0.

1116
01:56:45,760 --> 01:56:48,020
0, 1 genera re dos.

1117
01:56:48,800 --> 01:56:53,680
El conjunto C prima que es 1 sobre reis de 2, 1 sobre reis de 2.

1118
01:56:55,500 --> 01:57:00,520
En los 1 sobre reis de 2 y 1 sobre reis de 2 también genera re dos.

1119
01:57:01,700 --> 01:57:02,180
Moraleja.

1120
01:57:04,400 --> 01:57:07,020
Los generadores de una espacio en general no son únicos.

1121
01:57:08,640 --> 01:57:09,360
No van a ser únicos.

1122
01:57:09,440 --> 01:57:11,420
puede haber más de un conjunto que genere.

1123
01:57:12,150 --> 01:57:16,340
Y en general van a haber infinitos porque se usaban que se yo.

1124
01:57:16,520 --> 01:57:19,460
Este y este también generan y así siguiendo.

1125
01:57:20,440 --> 01:57:23,300
Cualquier par de vectores de erredos que no sean colineales

1126
01:57:23,820 --> 01:57:27,080
van a generar erredos, en el sentido de que cualquier

1127
01:57:27,220 --> 01:57:29,660
vector de erredos se puede escribir como combinación

1128
01:57:29,780 --> 01:57:30,320
lineal de ellos.

1129
01:57:32,160 --> 01:57:32,480
Bien.

1130
01:57:34,140 --> 01:57:36,280
Y por último, hay otro concepto que es crucial,

1131
01:57:36,400 --> 01:57:41,920
que es el de independencia lineal o dependencia lineal, lo pueden definir de distintas maneras,

1132
01:57:42,140 --> 01:57:49,300
pero dado un espacio vectorial B sobre Rc decimos que el conjunto C es linealmente independiente,

1133
01:57:50,410 --> 01:57:56,300
si siempre que tengo una combinación lineal igualada a cero, entonces todos los coeficientes

1134
01:57:56,300 --> 01:58:02,080
de la combinación lineal tienen que ser iguales a cero. Vamos a ver primero la motivación

1135
01:58:03,080 --> 01:58:04,700
y después hago unos cuentos.

1136
01:58:16,199 --> 01:58:17,300
Los vectores.

1137
01:58:21,340 --> 01:58:23,180
El R3 lo voy a hacer al ejemplo.

1138
01:58:23,980 --> 01:58:25,620
1 0 0, este acá.

1139
01:58:27,080 --> 01:58:29,320
Y acá vamos a graficar el 0 1 0.

1140
01:58:31,260 --> 01:58:34,040
y acá vamos a graficar el 001

1141
01:58:36,540 --> 01:58:38,860
ahora me aconsejaron un tercer vector que es el

1142
01:58:43,800 --> 01:58:44,480
el 120

1143
01:58:46,160 --> 01:58:47,060
que está en el plano

1144
01:58:47,940 --> 01:58:48,620
120

1145
01:58:49,920 --> 01:58:50,200
bien

1146
01:58:52,000 --> 01:58:52,600
120

1147
01:58:55,760 --> 01:58:56,380
este conjunto

1148
01:58:59,380 --> 01:59:00,060
120

1149
01:59:00,060 --> 01:59:05,620
y 1, 0, 0 no son linealmente independientes.

1150
01:59:06,640 --> 01:59:09,960
¿Por qué? Porque yo puedo dar una combinación lineal,

1151
01:59:23,000 --> 01:59:29,540
tal que se devuelva 0, pero que alfa, beta y gama no sean 0 todos al mismo tiempo.

1152
01:59:29,540 --> 01:59:44,300
tiempo, voy a poner precisamente si tomo alfa igual a 1, beta igual a -2 y gama igual a -1

1153
01:59:44,760 --> 01:59:52,880
entonces lo de arriba se hace cero y alfa, beta y gama no son todos ceros al mismo tiempo,

1154
01:59:55,060 --> 02:00:06,920
sin embargo, este conjunto, el 1, 0, 0, 0, 1, 0, 1 y 0, 0, 1 sí es linealmente independiente

1155
02:00:07,080 --> 02:00:14,660
porque se haga alfa por 1, 0, 0, más beta por 0, 1, 0 más gamma por 0, 0, 1.

1156
02:00:14,920 --> 02:00:18,400
La única forma de que esto sea cero es que

1157
02:00:22,840 --> 02:00:25,780
alfa se iguala beta, se iguala dama y se iguala cero.

1158
02:00:27,220 --> 02:00:28,680
¿Qué pasó? Bien.

1159
02:00:30,800 --> 02:00:37,060
En el primer ejemplo, el 1, 0, 0, el 1, 2, 0 y el 0, 1, 0 son coplanares.

1160
02:00:37,320 --> 02:00:38,560
Están los tres en el mismo plano.

1161
02:00:41,480 --> 02:00:44,060
Si son coplanares, son linealmente dependientes.

1162
02:00:44,060 --> 02:00:52,580
es decir, si hay tres en un plano van a ser linealmente dependientes. En cambio, como

1163
02:00:52,660 --> 02:01:00,040
el 0 1 0 1 no está en el plano de 1 0 0 y 0 1 0 1 0, esos van a ser linealmente independientes.

1164
02:01:00,200 --> 02:01:07,200
Entonces, la independencia lineal quiere decir que es un conjunto tal que ningún vector del

1165
02:01:07,240 --> 02:01:11,140
conjunto se puede escribir como combinación lineal de los otros vectores del conjunto.

1166
02:01:13,060 --> 02:01:16,780
Y es muy importante ese concepto en los espacios vectoriales.

1167
02:01:16,800 --> 02:01:17,900
¿Por qué? Porque...

1168
02:01:19,610 --> 02:01:21,780
Y ahora viene algo fundamental que,

1169
02:01:22,170 --> 02:01:27,800
tal un espacio vectorial B sobre los números reales o complejos,

1170
02:01:28,840 --> 02:01:30,900
decimos que el conjunto es una base,

1171
02:01:31,960 --> 02:01:35,760
si B es linealmente independiente y al mismo tiempo genera B.

1172
02:01:37,060 --> 02:01:40,860
Y la dimensión de un espacio vectorial va a venir dada

1173
02:01:40,860 --> 02:01:48,620
por el número de elementos de cualquiera de sus bases. Entonces no es sorprendente pero

1174
02:01:55,420 --> 02:02:07,219
les dejo como ejercicio probar que en R3 si tomamos B igual a 1, 0, 0, 0, 1, 0 y 0, 0, 1

1175
02:02:11,579 --> 02:02:22,680
este conjunto es linealmente independiente y genera, genera el retrés, entonces esto

1176
02:02:22,680 --> 02:02:28,440
es una base, entonces la dimensión de retrés es tres porque una base de retrés tiene tres

1177
02:02:28,500 --> 02:02:39,020
elementos. Ahora, las bases no son únicas, típicamente en los casos que vamos a ver

1178
02:02:39,160 --> 02:02:44,040
nosotros van a haber infinitas bases diferentes y no hay nada especial en ninguna base.

1179
02:02:45,300 --> 02:02:54,940
¿Cómo se interpreta eso geométricamente? Bueno, piensen que yo genero todo con, tengo una base

1180
02:02:54,940 --> 02:03:04,780
con estos tres de acá, ¿no? 1 0 0 0 0 1 0 y 0 0 1. ¿Qué pasa si esto lo roto? Si en vez de tener esos tengo que yo...

1181
02:03:07,760 --> 02:03:13,540
Ahí tengo otra base, roto sobre el eje z o lo podría haber rotado a esta terna,

1182
02:03:15,220 --> 02:03:26,400
si este lo llamamos e0, e1 y e2, a esta terna de 0 y 1 y 2 la podría derrotar en cualquier dirección

1183
02:03:28,000 --> 02:03:34,080
y vale todo lo mismo porque geométricamente es fácil darse cuenta de que uno puede hacer

1184
02:03:34,480 --> 02:03:38,420
exactamente las mismas consideraciones en cualquier dirección, entonces en particular

1185
02:03:38,540 --> 02:03:45,980
R3 va a tener infinitas bases, pero todas las bases de R3 van a tener común que tienen todas tres

1186
02:03:46,100 --> 02:03:57,460
elementos, y la dimensión, así como la dimensión de R3 es 3, no es difícil probar que la dimensión

1187
02:03:57,460 --> 02:04:08,920
de R4, es igual a 4 y pregunto ¿Cuál es la dimensión de C3?

1188
02:04:12,880 --> 02:04:19,980
Eso es una pregunta espinosa porque hay que pensar, hay que preguntarse qué quiero decir con C3, ¿no?

1189
02:04:24,020 --> 02:04:26,240
¿Cuánto dicen que es la dimensión de C3?

1190
02:04:29,800 --> 02:04:36,280
La que compre de un poco acá. La dimensión de Rm va a ser igual a N.

1191
02:04:40,380 --> 02:04:43,540
¿Hay alguien ahí todavía conectado? ¿Y sería 3 o no?

1192
02:04:44,640 --> 02:04:48,340
¿Puede ser 18, profe? No, no es 18, es 3.

1193
02:04:49,460 --> 02:05:19,440
¿Qué es el cuerpo que

1194
02:05:19,460 --> 02:05:26,320
vamos a tomar a CN como un espacio vectorial sobre los números complejos

1195
02:05:30,000 --> 02:05:34,580
entonces por qué esto es así bueno porque cómo es un vector de c a la n

1196
02:05:36,660 --> 02:05:47,180
si b está en c a la n b se escribe como alfa 1 tata alfa n donde los alfa y son numeritos complejos

1197
02:05:51,900 --> 02:05:59,840
¿Y cómo podemos armar una base de C al AN? ¿Una base de C al AN? Podemos hacer así, podemos

1198
02:06:00,040 --> 02:06:15,060
tomar el 1, 0, 0, 0, 0, ¿no? ¿Cómo? 0, 1, 0, 0, 0, 0, ¿no? ¿Cómo?

1199
02:06:17,180 --> 02:06:25,000
en particular porque como decían antes por ahí que si el cuerpo son los números complejos

1200
02:06:25,480 --> 02:06:36,560
yo puedo multiplicar a estos elementos, ya vemos les 0, E1, EN, los puedo multiplicar por

1201
02:06:37,540 --> 02:06:42,920
pasar suma de alfa y por EI, donde los alfa y son números complejos.

1202
02:06:45,180 --> 02:06:50,100
y entonces con esto me voy a poder armar cualquier vector de CN

1203
02:06:51,300 --> 02:06:55,540
de la dimensión de los complejos ananes para nosotros va a ser N

1204
02:06:56,420 --> 02:06:56,680
¿Está bien?

1205
02:07:05,160 --> 02:07:06,980
Bien, sigo

1206
02:07:14,300 --> 02:07:18,440
Bueno, y hoy no lo vamos a ver, pero se los voy adelantando.

1207
02:07:19,210 --> 02:07:20,720
Ya me lo preguntaban hace un rato, ¿no?

1208
02:07:26,520 --> 02:07:33,260
La evolución temporal de un estado va a venir dada por la multiplicación por una matriz.

1209
02:07:37,740 --> 02:07:39,920
La gracia es que esto va a ser geométrico, ¿no?

1210
02:07:40,500 --> 02:07:46,180
supongo que, es decir, en cuántica no vamos a usar espacios reales, pero bueno, para fijar ideas un poco

1211
02:07:47,180 --> 02:07:49,220
consideremos un espacio real.

1212
02:07:53,580 --> 02:07:58,740
Supongo que al inicio tiene el vector 1, 0, el sistema está en el estado 1, 0.

1213
02:08:00,070 --> 02:08:06,600
Y entonces para hacerlo evolucional en el tiempo, va a tener que hacerle algo, va a cambiar en el tiempo del estado.

1214
02:08:08,140 --> 02:08:13,800
En física cuántica la evolución va a venir dada por la multiplicación por una operada

1215
02:08:13,840 --> 02:08:20,320
lineal, por una matriz. Entonces tienen que multiplicar por una matriz. Entonces si multiplican

1216
02:08:20,320 --> 02:08:24,780
por esta matriz tienen por ejemplo que el vectorcito cambia de esta manera. Ah, y otra

1217
02:08:24,900 --> 02:08:37,320
cosa antes de continuar. Ven que me olvide decir. ¿Cuál es la dimensión de R a la n

1218
02:08:37,320 --> 02:08:46,420
por m, o sea, cuál es la dimensión del espacio de matrices de n por m y bueno, que va a ser claro,

1219
02:08:46,640 --> 02:08:54,020
n por m, ¿por qué? porque se puede dar una base así que tenga por ejemplo, vamos la de 2 por 2,

1220
02:08:54,020 --> 02:08:58,260
para que se vea, puedo hacer 1 0 0 0

1221
02:09:02,480 --> 02:09:04,000
0 1 0 0

1222
02:09:06,260 --> 02:09:09,180
0 0 0 1 0 y 0 0 0 1

1223
02:09:12,740 --> 02:09:17,040
y esta también sirve para el caso complejo porque si me permito multiplicar por

1224
02:09:17,120 --> 02:09:23,300
escalares complejos con estas cuatro matrices me voy a poder armar todas las matrices complejas

1225
02:09:25,680 --> 02:09:26,080
bien entonces

1226
02:09:28,720 --> 02:09:32,580
hasta acá tienen como para ver en el libro de Nielsen Chong

1227
02:09:36,060 --> 02:09:38,060
yo lo que les dejo como ejercicio es

1228
02:09:39,600 --> 02:09:42,360
lean la parte de Algebre la lineal del libro de Nielsen Chong

1229
02:09:42,540 --> 02:09:46,880
¿por qué? bueno porque el plan de la materia es que lean mucho

1230
02:09:47,520 --> 02:09:52,300
todo lo más que no van a llegar obviamente a leerlo todo porque es muy largo

1231
02:09:52,900 --> 02:09:55,340
pero que lean lo más que puedan del libro en el centro.

1232
02:09:55,600 --> 02:10:01,120
Y para eso se tiene que familiarizar con la notación y con la forma de razonamiento del libro.

1233
02:10:01,520 --> 02:10:08,300
Ven acá a los vectores complejos, los representan como una columna, como hice yo en mis diapositivas,

1234
02:10:08,560 --> 02:10:10,840
una columna z1 zn.

1235
02:10:12,220 --> 02:10:17,840
Acá les dice cómo sumar vectores, acá les dice cómo multiplicarlos por escalares.

1236
02:10:20,780 --> 02:10:35,840
Y yo les digo, si no saben inglés, traduzcan, traduzcan con Google Translate, es muy fácil. Hoy, hace, cuando yo estudiaba, había que luchar contra el inglés, pero bueno, hoy es muy fácil traducir.

1237
02:10:37,400 --> 02:10:42,880
y acá explican todo esto por ahí hay unas cosas no las van a entender yo les voy a dar también la

1238
02:10:42,880 --> 02:10:52,180
guía de ejercicios algunas y algunas cositas introductorias bueno y ahí tienen así que

1239
02:10:52,520 --> 02:11:00,960
ya vayan acostumbrándose al leer el libro es muy difícil o imposible avanzar en estos temas

1240
02:11:00,960 --> 02:11:08,380
avanzados o cosas tecnológicas avanzadas si si ustedes no leen los libros es muy

1241
02:11:08,460 --> 02:11:13,020
importante acostumbrarse a leer libros a tener paciencia a

1242
02:11:14,980 --> 02:11:19,380
encontrarse con que no se entiende nada entonces hay que pensar y hay que ver

1243
02:11:19,380 --> 02:11:24,960
las cosas una y otra vez bueno acostúmense bueno y otra cosa importante es

1244
02:11:25,620 --> 02:11:30,940
repasar las propiedades de los números complejos yo les había dicho que vamos a

1245
02:11:30,940 --> 02:11:33,620
hay unos conceptos ahora de los números complejos.

1246
02:11:35,440 --> 02:11:41,240
Habíamos dicho que un complejo era z, igual a a + b por i, con a y b números peores.

1247
02:11:43,540 --> 02:11:46,420
Otra cosa importante es el conjugado de un z.

1248
02:11:53,020 --> 02:11:58,760
Habíamos dicho que a los complejos se les podía pensar como reos,

1249
02:12:00,140 --> 02:12:02,080
al menos para hacer un dibujito

1250
02:12:03,800 --> 02:12:07,820
y entonces si z es igual a a + b por i

1251
02:12:09,460 --> 02:12:13,880
el conjugado de z se define como a - b por i

1252
02:12:14,800 --> 02:12:17,200
le cambian el signo a

1253
02:12:22,439 --> 02:12:27,020
entonces geométricamente si este z es este z conjugado

1254
02:12:28,660 --> 02:12:32,000
porque cambia la componente "b"

1255
02:12:33,500 --> 02:12:35,160
pasa a ser -b

1256
02:12:37,260 --> 02:12:39,560
atención por ejemplo si escribo z como

1257
02:12:42,920 --> 02:12:46,780
3+2i z con jugado es 3-2i

1258
02:12:48,520 --> 02:12:51,760
y si escribo z igual a

1259
02:12:52,700 --> 02:12:54,620
5-2i

1260
02:12:54,620 --> 02:12:59,300
Entonces z con jugado, o menos 5 menos 2, z con jugado es menos 5,

1261
02:12:59,710 --> 02:13:05,460
la componente real queda igual y la componente compleja cambia, de signo, ok?

1262
02:13:08,160 --> 02:13:09,560
Entonces, ese es el conjugado.

1263
02:13:11,620 --> 02:13:11,840
Bien.

1264
02:13:15,320 --> 02:13:18,720
La otra cosa importante es, ya lo dijimos que y cuadrado es menos 1,

1265
02:13:18,870 --> 02:13:23,340
entonces siempre en cualquier fórmula que les aparezca y por y o y cuadrado,

1266
02:13:23,660 --> 02:13:31,140
siempre le pueden empezar por -1 o viceversa, siempre que tengan -1 los pueden reescribir como hipóric.

1267
02:13:32,500 --> 02:13:39,620
Después, vinculada a esta representación geométrica de los complejos,

1268
02:13:40,240 --> 02:13:46,520
es decir, como vectores de R2, podemos calcular el módulo de un número complejo.

1269
02:13:47,180 --> 02:13:49,340
El módulo va a ser la longitud de este vector.

1270
02:13:50,020 --> 02:13:57,260
Bueno, si usamos pitágoras, esto, la del eje x, mi idea, y la del eje y, mi de b.

1271
02:13:57,960 --> 02:14:02,540
Entonces esto de acá arriba, mi de... se acuerdan, ok?

1272
02:14:02,960 --> 02:14:06,060
Por pitágoras cuando tenían un terécano de octángulo, sí.

1273
02:14:08,860 --> 02:14:11,640
A cuadrado más b cuadrado, el igual a c cuadrado, sí.

1274
02:14:12,860 --> 02:14:15,660
Entonces esto de acá, mi de...

1275
02:14:15,660 --> 02:14:19,640
el módulo de z, que sería la diagonal, sería

1276
02:14:21,460 --> 02:14:26,320
es la raíz cuadrada de a cuadrado más b cuadrada, ¿sí?

1277
02:14:28,840 --> 02:14:29,060
¿Sabes?

1278
02:14:29,920 --> 02:14:31,600
Esto es lo que puse acá en la diapositiva.

1279
02:14:34,000 --> 02:14:37,040
El módulo de z cuadrado es raíz de a cuadrado más b cuadrado.

1280
02:14:37,920 --> 02:14:39,360
Y el módulo de z cuadrado

1281
02:14:44,440 --> 02:14:45,640
coincide con

1282
02:14:46,960 --> 02:14:56,100
Z por Z con jugado, puedes hacer la cuenta, entonces A + B por I por A - B por I, cuando

1283
02:14:56,200 --> 02:15:06,540
haces esto le queda A por A a cuadrado, si me coligo, la vez, a cuadrado, después le queda

1284
02:15:07,360 --> 02:15:13,640
menos a por b por i y ahora más b por i por a y después

1285
02:15:14,940 --> 02:15:21,780
menos b por b y cuadrado y esto por último es acuadrado, este término se va

1286
02:15:21,780 --> 02:15:29,520
con este y cuadrado es -1 menos por menos más acuadrado, entonces el módulo del

1287
02:15:29,640 --> 02:15:33,860
complejo al cuadrado es z por z aconjugado

1288
02:15:34,280 --> 02:15:39,780
que coincide con a cuadrado más b cuadrado. Todas estas son cositas que tienen que tener

1289
02:15:40,740 --> 02:15:49,780
en mente. Es importante que refresca en todo esto, por eso se los estoy contando ahora.

1290
02:15:50,640 --> 02:15:56,480
Y si no lo vienen nunca, bueno aún más. Y todavía, todavía pueden usar esta notación,

1291
02:15:56,500 --> 02:16:02,820
porque si tienen la representación geométrica de los complejos en el plano

1292
02:16:03,620 --> 02:16:09,420
motiva a dar una representación con ángulos y con módulo.

1293
02:16:09,940 --> 02:16:11,240
Miren, cómo sería eso.

1294
02:16:20,780 --> 02:16:23,700
Tenemos que el z es a +/-.

1295
02:16:25,700 --> 02:16:26,160
bien

1296
02:16:29,700 --> 02:16:34,139
pero a si este ángulo lo llama antita

1297
02:16:38,179 --> 02:16:41,160
anteriormente ustedes saben, si no lo saben se los digo yo ahora

1298
02:16:42,099 --> 02:16:45,280
si este ángulo es tita y esto mide a y esto mide b y esto mide c

1299
02:16:55,220 --> 02:16:58,040
V sobre C es igual al coseno de Tita.

1300
02:17:05,680 --> 02:17:09,620
No, A sobre C es el coseno de Tita.

1301
02:17:11,820 --> 02:17:12,760
me confundí

1302
02:17:17,420 --> 02:17:19,559
A sobre B, A sobre C

1303
02:17:21,760 --> 02:17:23,900
A sobre C es igual al coseno de Tita

1304
02:17:25,840 --> 02:17:28,660
lo pueden definir así al coseno de Tita

1305
02:17:30,280 --> 02:17:32,460
y B sobre C es el seno de Tita

1306
02:17:35,160 --> 02:17:44,280
y se hacen ver sobre A es igual a la tangente de tita que es el seno de tita sobre coseno de tita

1307
02:17:47,080 --> 02:17:54,059
¿Cómo son las funciones seno de tita y coseno de tita? Si no lo saben repasenlas, el seno de tita es así

1308
02:17:54,300 --> 02:18:01,800
cena del piso de la cera 0, cena del piso de la cera 2 es 1, cena del piso de la cera 0 y así

1309
02:18:02,019 --> 02:18:06,219
siguiendo, son periódicas al infinitum.

1310
02:18:09,900 --> 02:18:12,019
El coseno es lo mismo pero está desfasado.

1311
02:18:17,360 --> 02:18:18,500
Eso es un función de títano.

1312
02:18:21,940 --> 02:18:24,980
en coseno coseno 0 es 1 coseno piso 0 es 0

1313
02:18:27,279 --> 02:18:29,179
no me quedan muy bien el dibujo pero

1314
02:18:30,179 --> 02:18:31,460
esa lo puedo buscar en cualquier lado

1315
02:18:31,550 --> 02:18:34,880
en cualquier lado está explicado lo que son las funciones de semi-coseno

1316
02:18:35,360 --> 02:18:37,719
acá lo tienen que refrescar, yo se los acabo de explicar

1317
02:18:39,580 --> 02:18:41,380
pueden tomar la definición así

1318
02:18:42,660 --> 02:18:45,540
la cuestión es que

1319
02:18:48,540 --> 02:18:55,800
La cuestión es que usando eso, ahora voy a poder tener una representación con ángulo

1320
02:18:55,900 --> 02:19:01,420
complejo, porque esta longitud acá, la diagonal esta, es el módulo de zeta.

1321
02:19:03,260 --> 02:19:08,500
Y entonces yo puedo escribir a A como módulo de zeta por el coseno de tita.

1322
02:19:10,420 --> 02:19:13,880
Y a B como módulo de zeta por el seno de tita.

1323
02:19:18,059 --> 02:19:36,240
Bien, entonces, entonces, z era a + b por i, esto es, módulo de z por coseta de tita + módulo de z por el seno de tita por i

1324
02:19:40,059 --> 02:19:47,740
y entonces saco factor como módulo de z por coseno de tita más y por el seno de tita

1325
02:19:50,240 --> 02:19:50,420
bien

1326
02:19:53,180 --> 02:19:58,040
y a esto de acá lo voy a definir como e alaí por tita

1327
02:20:00,561 --> 02:20:07,619
y entonces si defino así obtengo que z se puede escribir como módulo de z por e alaí tita

1328
02:20:08,120 --> 02:20:11,820
siempre teniendo en cuenta que "eala y tita" es igual a "coseno de tita"

1329
02:20:13,040 --> 02:20:15,160
más "i" por el seno de tita

1330
02:20:19,720 --> 02:20:21,160
¿Por qué esto es importante?

1331
02:20:21,400 --> 02:20:22,640
Bueno, porque a veces...

1332
02:20:26,420 --> 02:20:27,960
porque a veces simplifica las cuentas

1333
02:20:27,960 --> 02:20:32,060
o si tienen "w" igual a "modulo de w" por "eala y"

1334
02:20:32,380 --> 02:20:34,040
"an" de "w" que podrás hacer "fi"

1335
02:20:35,780 --> 02:20:45,020
entonces se hace el z por wb, esto es módulo de z por módulo de wb, e ala y tita por e ala y fin

1336
02:20:45,640 --> 02:20:50,000
y estas tienen la misma propiedad que el exponencial, entonces les queda módulo de z por wb

1337
02:20:50,520 --> 02:21:00,120
ah, acá no lo aclaré, acá uso que módulo de z por wb, es igual a módulo de z por módulo de wb

1338
02:21:00,120 --> 02:21:08,660
esto lo pueden chequear y esto me queda el ahí "titamafi" es como esto lo

1339
02:21:08,760 --> 02:21:13,180
pueden probar entonces la mania pueden hacer las cuentas usando las propiedades

1340
02:21:13,220 --> 02:21:15,860
de las funciones exterior y la métrica van a ver que esto es esa

1341
02:21:18,760 --> 02:21:23,060
¿Qué va a pasar en el curso? bueno que cada tanto yo voy a meter alguna cuentita

1342
02:21:23,070 --> 02:21:26,940
de estas porque vamos a hacer algún algoritmo cuántico y yo voy a sacar factor

1343
02:21:26,940 --> 02:21:29,600
como una fase, podríamos multiplicar fases.

1344
02:21:30,580 --> 02:21:36,820
Y bueno, si no tienen, si no están duchos con esto,

1345
02:21:36,920 --> 02:21:38,020
no se van a perder.

1346
02:21:38,580 --> 02:21:43,300
Entonces mi sugerencia es que intenten repasar las propiedades

1347
02:21:43,420 --> 02:21:47,240
de los números complejos todos los que puedan.

1348
02:21:52,260 --> 02:21:58,020
Yo estuve viendo y el libro de Nielsen Chong está resuelto.

1349
02:21:58,360 --> 02:22:02,380
Tiene unos tipos, la gente que ellos estudiantes o los

1350
02:22:02,540 --> 02:22:06,900
ingenieradores que se dedicaron a resolver todos los ejercicios

1351
02:22:06,900 --> 02:22:08,280
de vida y Nielsen y Chong.

1352
02:22:09,380 --> 02:22:10,860
Creo que por ahí eso puede servirles.

1353
02:22:11,040 --> 02:22:12,560
Después se les voy a compartir.

1354
02:22:14,500 --> 02:22:15,920
No es oficial la solución.

1355
02:22:16,260 --> 02:22:19,060
Como no está chequeado, puede ser que algunos ejercicios estén

1356
02:22:19,120 --> 02:22:19,340
mal.

1357
02:22:20,500 --> 02:22:25,780
Yo estuve mirando y en general es también pero hay que tomarlos con pinza, pero creo que puede ser

1358
02:22:28,060 --> 02:22:34,280
puede ser de utilidad para muchos de ustedes, el hecho de que puedan usar los resueltos.

1359
02:22:37,739 --> 02:22:39,160
Pero bueno, entonces...

1360
02:22:42,100 --> 02:22:50,480
Ah, y esto, esto es muy importante, fíjense una cosa, el módulo de la, de la, de esta exponencial de

1361
02:22:50,480 --> 02:22:55,120
la itita es uno siempre eso lo puedo probar como lo probó

1362
02:23:02,620 --> 02:23:11,280
habíamos dicho z era módulo de z por e a la itita y este e a la itita era coseno de

1363
02:23:11,320 --> 02:23:19,880
tita más y por el seno de tita. Bien, el módulo de ala de tita es

1364
02:23:25,480 --> 02:23:33,320
el módulo del cuadrado si quieren, es el coseno del cuadrado de tita más el seno del cuadrado de tita.

1365
02:23:34,580 --> 02:23:36,840
Porque esto, esto así como está es un número complejo.

1366
02:23:40,720 --> 02:23:43,180
Este es un complejo. Ahora aplico la fórmula del módulo.

1367
02:23:44,800 --> 02:23:48,840
En general, el cuadrado acá se pone, acá para que no haya ambiguidad de este no importa.

1368
02:23:49,240 --> 02:23:51,660
Vamos a dejarlo así. Vamos a poner para el entecito.

1369
02:23:53,940 --> 02:23:55,200
La obsesión. Bien.

1370
02:23:56,380 --> 02:23:59,060
Esto es una identidad trigonométrica y siempre vale 1.

1371
02:23:59,320 --> 02:24:02,340
De las funciones trigonométricas sale que esto siempre vale 1.

1372
02:24:02,520 --> 02:24:03,400
¿Por qué? Bueno, ¿por qué?

1373
02:24:07,840 --> 02:24:13,980
que arden el triángulo rectángulo del lado 1, esto mide raíz de 2 ¿no?

1374
02:24:16,540 --> 02:24:28,100
Es un vector, un vector que está en el círculo de raíz de 1, perdón, nada que ver con la rejera, ahí

1375
02:24:28,560 --> 02:24:33,540
Si tienen tita, esta proyección es el coseno y esta proyección es el seno.

1376
02:24:34,390 --> 02:24:35,840
Y esa es el círculo de radio 1.

1377
02:24:37,500 --> 02:24:44,100
También podrían por ejemplo definir al círculo del radio 1 como e a la isi,

1378
02:24:44,440 --> 02:24:49,280
donde phi pertenece al conjunto que se llama 0,2 pi, ¿no?

1379
02:24:53,040 --> 02:24:53,920
Lo dejamos abierto.

1380
02:24:56,840 --> 02:25:01,500
Bueno, acá el matemático me va a castigar porque...

1381
02:25:02,400 --> 02:25:04,840
Está bien igual si lo cierro, ¿no? No, tengo redundancia.

1382
02:25:07,300 --> 02:25:08,780
Bueno, no importa.

1383
02:25:11,770 --> 02:25:14,600
Lo importante es que esto tiene el módulo 1 y esto lo voy a usar.

1384
02:25:15,390 --> 02:25:19,760
Muy seguido me va a quedar que voy a obtener un vector.

1385
02:25:22,700 --> 02:25:30,100
voy a tener algo así como e ala i piso de 2 no sé lo que sea por una expresión y

1386
02:25:30,120 --> 02:25:34,460
voy a decir a éste y me lo salgo encima ¿por qué? porque es una fase global después

1387
02:25:34,490 --> 02:25:38,800
voy a explicar porque pero como éste va a tener módulo 1

1388
02:25:41,420 --> 02:25:47,720
lo vamos a descartar ok pero eso lo voy a explicar más adelante bien entonces

1389
02:25:47,720 --> 02:25:53,240
moraleza o conclusión tienen que repasar las propiedades de los números complejos. Yo lo acabo de

1390
02:25:53,320 --> 02:26:00,040
hacer el principio con esto deberían tener todo pero ¿qué va a pasar? Cuando tengan que

1391
02:26:00,080 --> 02:26:06,560
hacer cuentitas se les va a hacer matete si no hicieron muchas cuentitas de estas. Entonces bueno,

1392
02:26:07,380 --> 02:26:13,800
taten de estudiar esto de vuelta, de si pueden acceder al vídeo, ojala que se haya grabado la

1393
02:26:13,800 --> 02:26:19,860
que se ve. Si no lo vemos de vuelta, no se preocupen. La gracia de este curso es que es un curso

1394
02:26:20,340 --> 02:26:25,320
universitario, es largo y podemos volver a dar las cosas una y otra vez. Entonces yo voy a volver a

1395
02:26:26,380 --> 02:26:33,280
repetir las cuentas cuando vamos a saber los ritmos cuánticos y voy a explicar todo muy despacio y

1396
02:26:33,300 --> 02:26:38,600
ustedes me van a poder parar y yo les voy a poder explicar con lujo detalles todo. Que a diferencia

1397
02:26:38,600 --> 02:26:44,980
otros cursos está el problema de que uno está corriendo todo el tiempo y nunca tiene tiempo.

1398
02:26:48,580 --> 02:26:56,440
Bueno, ¿me escuchan por ahí, no? Sí. Sí, sí, sí, perfecto. Bien, pero tengan las

1399
02:26:56,620 --> 02:27:00,640
en mente a todas estas propiedades porque van a volver a una forma de...

1400
02:27:05,220 --> 02:27:10,060
Entonces les decía que después la otra cosa importante es en el curso va a ser

1401
02:27:10,240 --> 02:27:14,980
cómo se multiplica una matriz por un vector, supongo que tiene la matriz M que es

1402
02:27:15,240 --> 02:27:25,120
A, B, C, D y tiene el vector phi o psi que es alfa, beta. M por psi

1403
02:27:25,960 --> 02:27:31,040
por la matriz de un lado y el vector del otro y hay que hacer alguna cuenta o la

1404
02:27:31,040 --> 02:27:40,180
la cuenta es esta, en la primera coordenada del resultado tiene que hacer, la primera

1405
02:27:40,380 --> 02:27:45,860
mira, la primera fila de la matriz es a b y mira al vector como una columna, entonces

1406
02:27:45,880 --> 02:27:53,880
tiene que hacer a por alza más b por beta y lo ponen acá, y luego hacen lo mismo con

1407
02:27:53,880 --> 02:28:01,020
la segunda fila de la matriz y lo ponen la segunda coordenada, si tuvieran un vector

1408
02:28:01,020 --> 02:28:04,040
vector más grandes hacen una cuenta muy similar

1409
02:28:07,800 --> 02:28:10,180
entonces así se multiplica una matriz por vector

1410
02:28:10,740 --> 02:28:12,480
pero matrices vamos a ver la clase que viene

1411
02:28:12,760 --> 02:28:14,680
vamos a ver todo esto con más detalle

1412
02:28:18,460 --> 02:28:21,040
obviamente quienes ya ya han visto esto

1413
02:28:21,040 --> 02:28:22,520
lo pueden ir repasando

1414
02:28:26,320 --> 02:28:30,359
y al final cuando volviendo al comienzo de la clase

1415
02:28:30,360 --> 02:28:37,640
Habíamos dicho que estos vectores,

1416
02:28:38,250 --> 02:28:39,540
en los cuales estamos hablando,

1417
02:28:40,570 --> 02:28:44,400
en particular los vectores en un espacio vectorial complejo,

1418
02:28:44,880 --> 02:28:47,860
van a representar, ya veremos cómo, a los estados cuantos.

1419
02:28:49,140 --> 02:28:50,820
¿Y en qué sentido los representan? Bueno,

1420
02:28:52,760 --> 02:28:56,180
la idea es que el cero representa un estado posible,

1421
02:28:56,250 --> 02:29:00,080
por ejemplo, partícula atravesando la religión izquierda.

1422
02:29:00,780 --> 02:29:06,100
y el 1 representa otro estado, particular atrazando la rendija derecho.

1423
02:29:07,320 --> 02:29:12,560
Y la combinación lineal va a representar a los famosos gatos de Schrodinger.

1424
02:29:13,120 --> 02:29:16,020
Cuando da una combinación lineal entre 0 y 1,

1425
02:29:17,160 --> 02:29:21,840
lo que voy a hacer es estar describiendo un estado de superposición o de gato de Schrodinger.

1426
02:29:23,480 --> 02:29:26,880
Y lo que termina pasando es que los coeficientes de la combinación lineal,

1427
02:29:26,880 --> 02:29:29,480
si los números escalares que aparecen en la combinación ideal,

1428
02:29:29,690 --> 02:29:34,560
van a estar vinculados a la probabilidad de observar el resultado cero

1429
02:29:34,950 --> 02:29:36,700
o el resultado uno, respectivamente.

1430
02:29:37,880 --> 02:29:38,720
Esta va a ser la idea.

1431
02:29:39,740 --> 02:29:42,640
Obviamente, ahora le estoy explicando muy rápido y al pasar,

1432
02:29:44,300 --> 02:29:47,240
pero sobre esto profundizaremos en las próximas clases.

1433
02:29:47,480 --> 02:29:54,240
Pero justamente para entender esto o para poder manejarlo con soltura,

1434
02:29:54,680 --> 02:29:58,980
Es importante que se estudien las propiedades de los espacios vectoriales y del vector,

1435
02:29:59,399 --> 02:30:01,180
pues si no, no van a poder.

1436
02:30:02,500 --> 02:30:03,920
Lo van a entender, pero no tanto.

1437
02:30:05,300 --> 02:30:07,800
Y como estamos con tiempo y es la idea del curso,

1438
02:30:10,600 --> 02:30:13,040
uy, creo que eso fue que entró alguien, ¿no?

1439
02:30:13,180 --> 02:30:14,760
Sí, ahí está.

1440
02:30:21,020 --> 02:30:24,400
La verdad es que lo repasen así lo pueden entender de la mejor manera posible.

1441
02:30:24,580 --> 02:30:27,540
Pero la pregunta es ¿Qué es la probabilidad?

1442
02:30:28,280 --> 02:30:29,080
¿Qué es una probabilidad?

1443
02:30:29,280 --> 02:30:31,820
Sobre todo vamos a volver muchas veces en el curso.

1444
02:30:35,020 --> 02:30:37,760
¿Qué quiere decir si tira una moneda?

1445
02:30:38,060 --> 02:30:42,300
¿Qué quiere decir que la probabilidad de obtener cara es un medio?

1446
02:30:42,600 --> 02:30:44,160
Vamos a ver que es una moneda justa, ¿no?

1447
02:30:44,280 --> 02:30:45,480
No tiene ningún seco.

1448
02:30:46,520 --> 02:30:48,580
¿Qué quiere decir que la probabilidad es un medio?

1449
02:30:48,680 --> 02:30:50,300
alguien se anima a...

1450
02:30:50,300 --> 02:30:51,520
que sea el 2%

1451
02:30:53,140 --> 02:30:54,200
por ejemplo, claro

1452
02:30:54,240 --> 02:30:55,800
que lo que estoy a una cara con una luz

1453
02:30:56,800 --> 02:30:57,580
que de dos veces

1454
02:30:58,739 --> 02:30:59,700
una va a salir

1455
02:31:00,260 --> 02:31:01,820
hay dos estados posibles

1456
02:31:03,760 --> 02:31:04,220
va, para, para

1457
02:31:04,480 --> 02:31:06,820
está bueno porque todos dijeron cosas distintas

1458
02:31:07,280 --> 02:31:07,840
uno dijo

1459
02:31:09,100 --> 02:31:10,500
que sale cara con

1460
02:31:10,780 --> 02:31:11,240
50%

1461
02:31:12,180 --> 02:31:13,980
otro dijo que hay dos estados posibles

1462
02:31:14,540 --> 02:31:16,680
son todas cosas más o menos ciertas

1463
02:31:16,680 --> 02:31:25,860
posible si, cara o seca. Otro dijo que hay igual chance de que salga cara, que salga seca.

1464
02:31:29,479 --> 02:31:34,540
Y otro dijo que si la tiras dos veces una sale cara y otra está seca. Esa para mí está mal

1465
02:31:34,660 --> 02:31:40,060
porque podría pasar que yo tengo una moneda y la tiro dos veces y sale las dos veces cara.

1466
02:31:40,120 --> 02:31:43,660
la moneda, atención. Y que la

1467
02:31:47,820 --> 02:31:54,100
y tira la moneda diez veces y podría pasar que salga diez veces cara, ¿por qué no?

1468
02:31:54,580 --> 02:31:59,020
Pero si la espiritualidad finita es que va a salir siempre 50 veces.

1469
02:31:59,040 --> 02:32:04,280
Exacto, exacto, siempre, siempre, claro, pero no, igual es como...

1470
02:32:04,920 --> 02:32:06,180
pensemos, pensemos lo que pasaría.

1471
02:32:07,040 --> 02:32:10,820
Vamos a hacer una... una tal...

1472
02:32:12,820 --> 02:32:14,360
Ahí alguien dice...

1473
02:32:15,800 --> 02:32:19,920
Claro, va a tender a salir 50, 50, pero vamos a tratar de ponerle números a eso, porque eso

1474
02:32:20,620 --> 02:32:31,860
va a haber que lo vamos a tener que... va a pasar medio crucial para entender lo que pasa en los algoritmos cuánticos, porque el modelo de computación cuándo va a ser sí o sí proveniente.

1475
02:32:32,820 --> 02:32:41,980
bueno tengo la moneda ¿no? y acá voy a ir anotando cara o seca, esta es la tirada 1,

1476
02:32:42,640 --> 02:32:49,460
tirada 2, tirada 3, tirada 4 ¿se entiendes? voy a tirarnos 100 veces, bueno por ahí en la 1 sale

1477
02:32:49,540 --> 02:32:55,820
cara, en la 2 sale cara, en la 3 sale seca, la 4 sale cara, y así cara, seca, se entienden?

1478
02:32:57,900 --> 02:33:00,240
Entonces, ¿qué voy a contar?

1479
02:33:00,470 --> 02:33:02,960
La frecuencia de cara va a ser iguala.

1480
02:33:03,220 --> 02:33:06,620
La cantidad de veces que salió cara dividido 100,

1481
02:33:07,120 --> 02:33:08,260
que es el número de veces que la tiré.

1482
02:33:09,820 --> 02:33:13,220
Y la frecuencia de seca va a ser la cantidad de veces que salió

1483
02:33:13,400 --> 02:33:14,700
seca dividido 100.

1484
02:33:14,890 --> 02:33:15,760
¿Se entiende esta notación?

1485
02:33:17,660 --> 02:33:17,840
Sí.

1486
02:33:18,319 --> 02:33:22,000
Ahora, ahora, si yo lo hago esto, no lo voy a hacer

1487
02:33:22,100 --> 02:33:22,820
porque se me envole.

1488
02:33:22,970 --> 02:33:24,080
No voy a decirlo, si lo hago.

1489
02:33:25,220 --> 02:33:29,740
Pero si lo hiciera, ¿ustedes cuánto dirían que vale este y cuánto vale este?

1490
02:33:32,260 --> 02:33:34,040
Sí, si lo hiciera.

1491
02:33:36,020 --> 02:33:42,420
Podría ser que sea 50-50, que justo a la mitad de las veces sale a cara y justo a la mitad de las veces sale a secar.

1492
02:33:42,920 --> 02:33:49,680
Pero, no sé, para los físicos esto es medio una pelotudes, pero en realidad si lo hacen en concreto al experimento,

1493
02:33:50,520 --> 02:33:58,980
por ahí de las 100 tiradas no sale así por ahí sale 47 veces cara y 53 veces seca

1494
02:34:00,919 --> 02:34:10,140
por ejemplo, háganlo en la casa, tire en la moneda 10 veces y bueno de las 10 veces por ahí en una

1495
02:34:10,440 --> 02:34:16,920
haga una ronda de 10, en esa ronda de 10 por ahí sale 5 y 5, bueno pues se hace en una nueva ronda de 10

1496
02:34:16,920 --> 02:34:23,040
por el salen seis y cuatro o cuatro y seis o siete y tres se entiende o ocho y dos. Ahora claro,

1497
02:34:23,360 --> 02:34:33,420
obvio las tiradas si la moneda es justa, las tiradas que tienden el 50 a 50 son las más

1498
02:34:33,500 --> 02:34:39,620
usuales, es improbable que yo tire una moneda diez veces y que salga diez veces cara ¿no?

1499
02:34:40,840 --> 02:34:45,439
Puede pasar, puede pasar no está prohibido por las leyes de la física, bueno al final le

1500
02:34:45,440 --> 02:34:51,840
no, justo que salga diez veces no está prohibido por la ley de la asesina, puede pasar, tiene

1501
02:34:51,900 --> 02:34:56,920
una moneda diez veces y que salga diez veces seca o diez veces cara. Ahora lo que no puede

1502
02:34:57,040 --> 02:35:01,880
pasar es que si la moneda es justa la tire un número muy grande de veces y que salga

1503
02:35:01,920 --> 02:35:11,761
sin precar, ¿se entienden? Si la tiro un número muy grande de veces, si hago F, C igual a

1504
02:35:11,760 --> 02:35:21,980
cantidad de veces, de cara sobre n, sobre n, esto va a tener a 50, perdón, va a tener

1505
02:35:22,620 --> 02:35:29,700
a un medio cuando n es tiendo infinito, ¿se entiende? cuando n es tiendo infinito, la frecuencia

1506
02:35:29,930 --> 02:35:34,840
de veces con la que sale cara, ¿qué quiere decir infinito en un experimento? Bueno, n es

1507
02:35:34,880 --> 02:35:40,241
muy grande. Para una moneda 100 es un número lo suficientemente

1508
02:35:40,240 --> 02:35:47,500
grande y se hace el experimento va a dar bastante parecido a un medio, pero si lo hacen con el igual a 10

1509
02:35:49,380 --> 02:35:54,520
no siempre les va a dar parecido a un medio, se entiende? porque 10 no es mucho más grande que 2,

1510
02:35:54,750 --> 02:36:03,562
en la moneda tienen dos posibilidades, cara o seca. Cuando miren la frecuencia, la frecuencia sería

1511
02:36:03,560 --> 02:36:11,860
sería esto, empíricamente sería esto, hace las repeticiones, si el número de repeticiones

1512
02:36:12,710 --> 02:36:21,080
que hacen es muy pequeño, la frecuencia va a ser una aproximación tosca a la noción

1513
02:36:21,080 --> 02:36:27,020
de Provelian. El número de repeticiones tiene que ser lo suficientemente grande como para

1514
02:36:27,040 --> 02:36:30,300
que estas fluctuaciones, estas anomalías, ¿no?

1515
02:36:30,520 --> 02:36:33,160
Estas de que las tiras cinco veces y salen cinco veces cara,

1516
02:36:34,410 --> 02:36:36,660
se compense y no las veamos, ¿sí?

1517
02:36:38,860 --> 02:36:45,060
Entonces ahí volvamos a la definición de probabilidad.

1518
02:36:48,801 --> 02:36:50,340
¿Cómo definimos la probabilidad?

1519
02:36:50,500 --> 02:36:55,500
Como la frecuencia, ahí hay una, aunque no lo crean,

1520
02:36:55,560 --> 02:37:04,700
hay un debate muy grande en la... a ver, Dale Juan. Dale, Feo, yo tenía la duda porque

1521
02:37:05,620 --> 02:37:10,800
bueno, yo lo estaba viendo con profesor Poca y la fórmula esta es el número de casos

1522
02:37:11,060 --> 02:37:16,340
totales sobre, bueno, casos favorables y número de casos totales cuando es como caso

1523
02:37:16,420 --> 02:37:22,762
improbable. Entonces, yo quería preguntar, ¿el tipo de probabilidades que vamos a trabajar

1524
02:37:22,760 --> 02:37:26,520
puede ser equi probable o puede ser de cuestiones infinitas?

1525
02:37:27,860 --> 02:37:30,480
No, no, no, pueden no ser equi probables.

1526
02:37:31,160 --> 02:37:36,060
Justamente en cuántica pasa a tener monedas que va a ser 80-20.

1527
02:37:37,960 --> 02:37:38,860
Oh, ok, ok.

1528
02:37:40,260 --> 02:37:41,700
Pero la frecuencia se me da igual.

1529
02:37:42,000 --> 02:37:44,580
Vos cuando vas al experimento con el sistema cuántico vas a decir,

1530
02:37:44,760 --> 02:37:49,762
bueno, el spin de la partícula va a dar up con probabilidad 80%.

1531
02:37:49,760 --> 02:37:56,120
Y bueno, eso quiere decir que si haces el experimento mil veces, más o menos 800 veces te va a salir

1532
02:37:56,860 --> 02:37:59,680
spin up y más o menos 200, spin down.

1533
02:38:03,819 --> 02:38:11,380
Entonces esto nos lleva al concepto de que es la probabilidad, no es evidente,

1534
02:38:12,420 --> 02:38:17,960
porque por ejemplo, ahora probablemente yo vaya al supermercado, tengo que comprar conmigo.

1535
02:38:17,960 --> 02:38:24,720
Sí. Te tengo una pregunta. Por ejemplo, con el caso de la moneda, puede ser quizás que no sea 50-50

1536
02:38:24,940 --> 02:38:29,800
la probabilidad, ¿no? Que quizás... Sí, por supuesto que puede ser una moneda. Sí, más de un lado que el otro.

1537
02:38:29,800 --> 02:38:36,280
El efecto de la fábrica. Exacto, exacto, sí. Pero así todos podemos afirmar que es 50-50?

1538
02:38:37,460 --> 02:38:43,180
No, justamente. ¿Sólo por si tiene dos lados? No, no, justamente, no, justamente, no. Justamente.

1539
02:38:43,320 --> 02:38:49,860
el fabricante, si vas a un casino, supone que vas a un casino y un jugo de moneda y el tipo tira la moneda

1540
02:38:50,700 --> 02:38:55,740
el fabricante de la moneda la vende prometiendo que la prueba le va a hacer 50-50

1541
02:38:58,619 --> 02:39:03,440
sin embargo podría ser un casino fraudulento o que el fabricante que fabricó la moneda

1542
02:39:03,520 --> 02:39:10,643
es una mala moneda y la moneda tiene un sesgo, no es 50-50 por ahí es 55-45

1543
02:39:11,640 --> 02:39:18,040
Si existiera, si el apostador se da cuenta de que hay un sesgo podría intentar sacar ventaja del casino,

1544
02:39:18,400 --> 02:39:22,280
¿entendés? O el cupier que tira la moneda sacar ventaja del apostador.

1545
02:39:23,940 --> 02:39:31,740
Entonces, ¿cómo harías vos para determinar si una moneda es justa o no? O si un dado es justo o no?

1546
02:39:32,760 --> 02:39:35,280
Por ejemplo, si tiras un dado hay seis posibilidades.

1547
02:39:36,960 --> 02:39:44,720
Si lo tiras 100 veces, bueno, un sexto de 100 debería salir uno, otro sexto, ¿entendés?

1548
02:39:45,439 --> 02:39:50,560
Perdón, perdón, comprobaría un sexto, debería salir uno, comprobaría un sexto,

1549
02:39:50,580 --> 02:39:53,260
debería salir dos, comprobaría un sexto y así, todas las cartas.

1550
02:39:53,430 --> 02:39:54,600
Es el dado equiprobable.

1551
02:39:55,360 --> 02:40:00,560
Pero un dado real por ahí tiene un sesgo, porque está mal fabricado, ¿me entendés?

1552
02:40:01,580 --> 02:40:04,420
Entonces ¿cómo harías vos para medir la probabilidad de cara a cara?

1553
02:40:04,560 --> 02:40:08,000
Bueno, harías este experimento. Arras el lado.

1554
02:40:13,600 --> 02:40:18,260
Tenés. El lado sería cara 1, 2, 3, 4, 5, 6, ¿no?

1555
02:40:19,620 --> 02:40:22,080
Entonces, en la tirada 1, por ahí sale la cara 1.

1556
02:40:23,100 --> 02:40:24,900
En la tirada 2 sale la cara 3.

1557
02:40:25,440 --> 02:40:28,440
En la tirada 3, entonces, ya sí, tendrías una tabla.

1558
02:40:30,160 --> 02:40:37,300
Bueno, entonces, la frecuencia de uno sería la cantidad de veces que salió el número uno dividió el número de ideas totales.

1559
02:40:37,300 --> 02:40:43,120
La frecuencia de dos sería el número de veces que salió dos o el número total y así. Hasta la frecuencia de seis, ¿no?

1560
02:40:51,200 --> 02:40:57,240
Y entonces vos esto lo podrías medir, que vos podrías ver empíricamente cuánto valen estos numeritos,

1561
02:40:57,360 --> 02:41:02,620
o estimar, que sé yo, esto es una ciencia, esto es que, pero toscamente, vos podrías

1562
02:41:02,900 --> 02:41:09,180
hacer esto. Entonces, si es esto, idealmente tendría que haber un sexto, un sexto y un

1563
02:41:09,320 --> 02:41:13,980
sexto. Si te dan distinto de un sexto, vos decís, bueno, el lado está sesgado, ¿no?

1564
02:41:15,360 --> 02:41:19,520
Pero tenés que tener cuidado de tirarlo en una cantidad lo suficientemente grande de

1565
02:41:19,660 --> 02:41:21,780
veces como parte de una muestra estadística robusta.

1566
02:41:27,461 --> 02:41:34,240
Bueno, tenía un poco más de esto pero me parece que está bueno ir lento.

1567
02:41:36,340 --> 02:41:38,580
Y hoy ya más o menos es la hora. ¿Hay alguna pregunta?

1568
02:41:44,700 --> 02:41:45,760
Ya tengo una pregunta.

1569
02:41:49,360 --> 02:41:59,500
¿Existe una posibilidad que sea ridículamente remoto de que haya una tercera posibilidad en mes de un 50% o otro 50%?

1570
02:42:02,200 --> 02:42:13,220
En el caso de la moneda, no. Eso queda definido por el sistema. Si vos te concentras en los eventos cara y seca, es porque no hay un tercer evento.

1571
02:42:13,960 --> 02:42:15,800
- Ok, no, no... - Pero...

1572
02:42:16,240 --> 02:42:19,540
- Probablemente que cayo de perfil o no... - Pero, pero, no...

1573
02:42:20,000 --> 02:42:25,100
Justamente vos podrías si, podrías... te le iba a decir... vos podrías ir, bueno, pero yo que sé,

1574
02:42:25,840 --> 02:42:31,580
quien sabe, por ahí la tiró y se alirian toda la planeta, para que caiga, viste, y queda parada.

1575
02:42:33,200 --> 02:42:39,020
De locos, pero, bueno, ahí vos deberías incluir ese evento, como posible.

1576
02:42:39,520 --> 02:42:42,282
- A la cosa. - Sabría cara seca y...

1577
02:42:42,680 --> 02:42:43,820
y paradas, ¿no?

1578
02:42:44,640 --> 02:42:47,620
Lo que pasa es que, típicamente, si vos lo incluís,

1579
02:42:48,320 --> 02:42:50,700
la probabilidad de que caiga parada es nula.

1580
02:42:52,060 --> 02:42:52,500
Entende.

1581
02:42:52,980 --> 02:42:57,200
En cualquier experimento que hagas, te va a dar que la frecuencia de que caiga parada es 0 siempre,

1582
02:42:57,300 --> 02:42:58,680
todo es igual, es probabilidad 0.

1583
02:42:59,250 --> 02:43:03,520
Y ojo que yo esto lo estoy explicando, lo estoy contando así como toscamente,

1584
02:43:03,720 --> 02:43:05,240
pero esto es todo un área de investigación.

1585
02:43:05,620 --> 02:43:06,780
¿Cómo definir probabilidad?

1586
02:43:07,210 --> 02:43:10,520
¿Y cómo definir eventos de probabilidad nula?

1587
02:43:11,120 --> 02:43:17,500
porque el que dijimos recién, por ejemplo, también podría pasar que un evento, esto del

1588
02:43:17,680 --> 02:43:23,000
matemático también puede, seguro que vos lo viste, un evento podría tener probabilidad en una y aún

1589
02:43:23,100 --> 02:43:32,580
así que pase una vez. Una vez en toda la edad del universo. Y aún así va a tener probabilidad en una.

1590
02:43:32,640 --> 02:43:33,080
¿Tenés?

1591
02:43:33,740 --> 02:43:35,280
Sería no lo podemos hacer.

1592
02:43:36,560 --> 02:43:41,740
Claro, porque tenés que tener cuidado entre el mundo real y el mundo matemático.

1593
02:43:42,400 --> 02:43:44,840
Vosotros es una definición matemática de probabilidad, ¿no?

1594
02:43:46,580 --> 02:43:46,900
Claro.

1595
02:43:47,560 --> 02:43:50,460
O sea, depende cómo definas el espacio de probabilidad,

1596
02:43:51,340 --> 02:43:55,980
después en que hares eventos de probabilidad nula, pero que podrían alguna así pasar.

1597
02:43:56,720 --> 02:43:59,880
Típicamente en física, si tienes probabilidad nula, no ocurre nunca, ¿no?

1598
02:43:59,880 --> 02:44:05,780
¿no? ¿sí, los físicos? Si, si entendés, si, si yo digo que tiene probabilidad c,

1599
02:44:05,960 --> 02:44:13,760
que no va a pasar nunca, por ejemplo, si, cuál es la probabilidad de salir volando ahora cero,

1600
02:44:13,940 --> 02:44:19,260
¿visto? No va a pasar jamás, ¿no? Pero lo que te quiero transmitir con esto es que el

1601
02:44:19,300 --> 02:44:25,120
concepto matemático de probabilidad es complejo, es complejo y da lugar a grandes debates en la

1602
02:44:25,160 --> 02:44:32,840
literatura. En particular, el concepto de probabilidad cuántica, pues fíjate que con el lado volvemos

1603
02:44:32,840 --> 02:44:36,600
a lo que discutíamos la vez pasada uno pensaba que el lado cuando lo tirabas

1604
02:44:38,560 --> 02:44:43,520
vos no sabes que cara va a caer porque no sabes todas las fuerzas que hay en juego

1605
02:44:43,910 --> 02:44:51,140
todas las fuerzas de rozamiento no sabes sin embargo la probabilidad que hay en cuántica

1606
02:44:51,260 --> 02:44:55,880
nosotros pensamos o algunos de nosotros físicos pensamos que no es por ignorancia sino que es

1607
02:44:55,920 --> 02:45:02,040
una probabilidad real es como una sarin trince con la naturaleza te lo pregunto de esta manera vos

1608
02:45:02,040 --> 02:45:07,960
pensar que todo está determinado en el mundo, por ejemplo, si vos ahora te vas a comer un choripán,

1609
02:45:08,780 --> 02:45:16,300
no? Si te termina la clase y te vas a morfalar un choripán. Y te lo... y vas y comés efectivamente

1610
02:45:16,400 --> 02:45:21,360
un choripán. Estás determinado a moverte ese choripán o hay opciones. O vos terminas la clase de

1611
02:45:21,420 --> 02:45:26,600
decir bueno, que quiero un choripán, o quiero ir a tomar un helado, o no quiero comer nada. Entendés?

1612
02:45:26,640 --> 02:45:34,660
y lo vas decidiendo. ¿Está determinado el futuro? Bueno, no, no sabemos, tendemos a creer que hay

1613
02:45:34,720 --> 02:45:40,480
opciones y que uno tiene la libertad de elegir entre las distintas opciones. Un libro de albedrío

1614
02:45:40,640 --> 02:45:47,020
hipotético. Claro, un libro de albedrío hipotético. No está en la red. Es que no lo sabemos, sí,

1615
02:45:47,720 --> 02:45:53,279
podría haber libro albedrío, ¿no? Y que también es complejo porque el hecho de que el mundo sea

1616
02:45:53,280 --> 02:45:56,800
probabilístico no garantiza tampoco que haya ayuda al oído. Es un quilombo.

1617
02:45:56,970 --> 02:46:04,500
Yo te hago una historia larga, corta. El punto sería que en el dado, si vos

1618
02:46:04,560 --> 02:46:08,320
pensás que el lado está gobernado por la leyes de la física clásica, no hay

1619
02:46:08,360 --> 02:46:17,300
posibilidades. Pues lo tirabas, nos vemos a ver, suerte, lo tirabas y el lado iba a

1620
02:46:17,400 --> 02:46:22,360
caer en cinco. Nos pasa que vos no sabías dónde iba a caer, porque no controlas

1621
02:46:22,360 --> 02:46:27,280
todas las variables. En cambio en cuántica nosotros queremos, o al menos una de las hipótesis

1622
02:46:27,570 --> 02:46:33,300
de Bonn, de Heisenberg y todas estas gente que es probabilística en la descripción, porque

1623
02:46:33,300 --> 02:46:40,060
es probabilístico el mundo. El electrón si va a pasar por izquierdo a la derecha no sabe,

1624
02:46:40,330 --> 02:46:44,620
no está determinado y en un momento se produce un evento izquierdo a derecha,

1625
02:46:46,680 --> 02:46:52,940
y la probabilidad mide la potencia de que ocurra eso, es como una medida de la tendencia a algo,

1626
02:46:53,360 --> 02:46:57,180
¿entendés? Eso después puedo volver, dando a Heisenberg, ¿viste?

1627
02:47:00,440 --> 02:47:06,740
Bueno, muchas gracias. Bueno, si vamos a cortemos por hoy y si vamos en contacto por

1628
02:47:08,380 --> 02:47:12,260
los distintos foros que tenemos, por ahora ya hay distintas, ya tenemos sus mails,

1629
02:47:12,260 --> 02:47:18,580
así que después les mando el recordatorio de la próxima clase y mañana les mando los ejercicios

1630
02:47:19,300 --> 02:47:23,780
para que pero igual ya saben que los de Niels y Chong tienen que leer eso lo tienen que leer

1631
02:47:26,439 --> 02:47:33,200
bueno gente, si quieren grabó por favor manden el video, compartanme el video, bueno, nos vemos, chao

1632
02:47:33,200 --> 02:47:33,660
-Tá bom,
```

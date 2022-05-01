# PiscaIdades
código que varia sobre determinado valor de idade. Feito para atividade de faculdade. ESP32 em mikropython

#Importar as bibliotecas de definições do pinos e biblioteca do tempo
from machine import Pin
from time import sleep

#Definir a função de cada pino que for usado
led1 = Pin(13, Pin.OUT)
led2 = Pin(12, Pin.OUT)
led3 = Pin(14, Pin.OUT)
led4 = Pin(27, Pin.OUT)
led5 = Pin(26, Pin.OUT)
led6 = Pin(25, Pin.OUT)
led7 = Pin(33, Pin.OUT)
led8 = Pin(32, Pin.OUT)
botaoVerde       = Pin(23, Pin.IN)
botaoVermelho    = Pin(22, Pin.IN)

#Inicializar as variáveis

#Agora vamos montar o programa principal
nasc = 2003 # ano do meu nascimento
ano = 2022 # ano que estamos

while(True):
  idade = ano - nasc
  print(idade)

  if(19 > idade >= 18):
    led1.value(1)
    sleep(0.5)
    led1.value(0)
    sleep(0.5)

  if(20 > idade >= 19):
    led1.value(1)
    led2.value(1)
    sleep(1)
    led1.value(0)
    led2.value(0)
    sleep(1)

 #idades respectivas...

  if(idade > 26):
    led1.value(1)
    led2.value(1)
    led3.value(1)
    led4.value(1)
    led5.value(1)
    led6.value(1)
    led7.value(1)
    led8.value(1)
    sleep(0.5)
    led1.value(0)
    led2.value(0)
    led3.value(0)
    led4.value(0)
    led5.value(0)
    led6.value(0)
    led7.value(0)
    led8.value(0)
    sleep(0.5)

   https://wokwi.com/projects/330410799959900754

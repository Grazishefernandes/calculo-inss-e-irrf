# calculo-inss-e-irrf
import math 
salario=int(input("digite o seu salario: "))
valevale=input("descontar o vale transporte?")
if salario <1320.01: 
  inss=salario*0.075
  print (f"calculo do INSS r${inss}")
  sl=(salario-inss)
  print ("Seu salario liquido é de: R$",salario)
elif salario >1320.01 and salario <2571.29:
  inss=(salario-1320.01)*0.09+99
  irrs= (salario*1320.01-158.40)
  print (f"calculo do imposto de renda R$:{irrs}")
  print (f"calculo do INSS R${inss}")
  sl=(salario-inss)
  print ("Seu salario liquido é de: R$ ",salario)
elif salario >2571.29 and salario <3856.94:
    inss=(salario-2571.29)*0.012+99+112.62
    print (f"calculo do INSS R${inss}")
    sl=(salario-inss)
    print ("Seu salario liquido é de: R$ ",salario)
elif salario <3856.95 and salario >7507.49:
    inss=(salario-3856.95)*0.014+99+112.62+154.28
    print(f"calculo do INSS R${inss}")
    sl=(salario-inss)
    print ("Seu salario é de: R$",salario)
elif salario >7507.49:
    inss =(salario-3856.95)*0.014+99+112.62+154.28+511.07
    print (f"Calculo do INSS R${inss}")
    sl=(salario-inss)
    print ("Seu salario liquído é de: R$", salario)
if salario == "s" or valevale == "S":
   valevale= (salario-inss)-valevale
   print(f"desconto de vale transporte é de: R${valevale}")
   print ("seu salario liquido é de: R$",salario)
irrf=float(input("digite o calculo:"))
if irrf <2112.00:
    irrf=(0.00)
    print("isento", (irrf))
elif irrf >2112.01 and irrf <=2826.65:
    irrf=(2112.01-170)-0.075
    print("calculo do IRRF",(irrf))
elif irrf >2826.65 and irrf <=3751.05:
    irrf=(2826.65-242.26)-0.015
    print("calculo do IRRF",(irrf))
elif irrf >3751.05 and irrf <=4664.68:
    irrf=(3751.05-353.19)-22.5
    print("calculo do IRRF",(irrf))
elif irrf >4664.68:
    irrf=(4664.68-478.97)-27.5
    print("calculo do IRRF",(irrf))
  
   

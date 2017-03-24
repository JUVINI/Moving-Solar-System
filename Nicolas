# --- Importation de Tkinter et des Maths --- #
from tkinter import *
from math import*


# --- Corps du programme --- #
fen=Tk()
fen.title("Système Solaire - Orbites planétaires telluriques")

largeurEcran=1400
hauteurEcran=700
miLEcran=largeurEcran/2
miHEcran=hauteurEcran/2

can = Canvas(fen, width = largeurEcran, height = hauteurEcran, bg = "black")
can.pack()



axe=can.create_line(0, miHEcran, largeurEcran, miHEcran, fill="white",dash=(4, 4))

imgSun = PhotoImage(file='/Users/Soleil.PNG')
can.create_image(miLEcran, miHEcran, image=imgSun)


can.create_text(miLEcran,miHEcran+20,text="Soleil",fill="white", activefill="yellow")



# --- Terre --- #

x,y, t = miLEcran-7,miHEcran+189, 0
terre= can.create_oval(x, y, x+14, y+14,fill='blue')
trajectoire = can.create_oval(miLEcran-196,miHEcran-196,miLEcran+196,miHEcran+196,outline='gray')
                        

# --- Fonction permettant d'animer un objet en lui faisant suivre une trajectoire circulaire uniforme --- #
def animeTerre():
   global x, y, t
   angle = radians(t)
   x = x + 3.42*cos(angle)
   y = y - 3.42*sin(angle)
   can.coords(terre,x,y, x+14,y+14)
   #print("A t=", t, ", on a xGterre =", x+7, "et yGterre =", y+7)
   t+=1
   fen.after(10,  animeTerre)
   if t==360:
      t=0


# --- Mars --- #

xMars, yMars, tM = miLEcran-4, miHEcran+295, 0
mars = can.create_oval(xMars, yMars, xMars+8, yMars+8, fill='red')
trajetoire = can.create_oval(miLEcran-299,miHEcran-299,miLEcran+299,miHEcran+299,outline='gray')


def animeMars():
   global xMars, yMars, tM
   angle = radians(tM)
   xMars = xMars + 5.22*cos(angle)
   yMars = yMars - 5.22*sin(angle)
   can.coords(mars,xMars,yMars, xMars+8,yMars+8)
   #print("A tM=", tM, ", on a xGMars =", xMars+4, "et yGMars =", yMars+4)
   tM+=1
   fen.after(10,  animeMars)
   if tM==360:
      tM=0

# --- Mercure --- #

xMercure, yMercure, tMe = miLEcran-3, miHEcran+67, 0
mercure = can.create_oval(xMercure, yMercure, xMercure+6, yMercure+6, fill='gray')
trajetoire = can.create_oval(miLEcran-70,miHEcran-70,miLEcran+70,miHEcran+70,outline='gray')


def animeMercure():
   global xMercure, yMercure, tMe
   angle = radians(tMe)
   xMercure = xMercure + 1.22*cos(angle)
   yMercure = yMercure - 1.22*sin(angle)
   can.coords(mercure,xMercure,yMercure, xMercure+6,yMercure+6)
   #print("A tMe=", tMe, ", on a xGMercure =", xMercure+3, "et yGMercure =", yMercure+3)
   tMe+=1
   fen.after(10,  animeMercure)
   if tMe==360:
      tMe=0

# --- Venus --- #

xVenus, yVenus, tV = miLEcran-6.8, miHEcran+135.2, 0
venus = can.create_oval(xVenus, yVenus, xVenus+6, yVenus+6, fill='yellow')
trajetoire = can.create_oval(miLEcran-142,miHEcran-142,miLEcran+142,miHEcran+142,outline='gray')


def animeVenus():
   global xVenus, yVenus, tV
   angle = radians(tV)
   xVenus = xVenus + 2.46*cos(angle)
   yVenus = yVenus - 2.46*sin(angle)
   can.coords(venus,xVenus,yVenus, xVenus+13.6,yVenus+13.6)
   #print("A tV=", tV, ", on a xGVenus =", xVenus+6.8, "et yGVenus =", yVenus+6.8)
   tV+=1
   fen.after(10,  animeVenus)
   if tV==360:
      tV=0

animeTerre()
animeMars()
animeMercure()
animeVenus()
fen.mainloop

      
window = Tk()
window.title("Système Solaire - Orbites planétaires gazeuses")

largeurEcran=1400
hauteurEcran=700
miLEcran=largeurEcran/2
miHEcran=hauteurEcran/2

canvas = Canvas(window, width = largeurEcran, height = hauteurEcran, bg = "black")
canvas.pack()

axe=canvas.create_line(0, miHEcran, largeurEcran, miHEcran, fill="white",dash=(4, 4))



'''
imgSoleil = PhotoImage(file='/Users/soleil2.PNG')
canvas.create_image(miLEcran, miHEcran, image=imgSoleil)

canvas.create_text(miLEcran,miHEcran+20,text="Soleil",fill="white", activefill="yellow")      
'''



# --- Jupiter --- #

xJupiter, yJupiter, tJ = miLEcran-10, miHEcran+60, 0
jupiter = canvas.create_oval(xJupiter, yJupiter, xJupiter+20, yJupiter+20, fill='orange')
trajetoire = canvas.create_oval(miLEcran-70,miHEcran-70,miLEcran+70,miHEcran+70,outline='gray')


def animeJupiter():
   global xJupiter, yJupiter, tJ
   angle = radians(tJ)
   xJupiter = xJupiter + 1.22*cos(angle)
   yJupiter = yJupiter - 1.22*sin(angle)
   canvas.coords(jupiter,xJupiter,yJupiter, xJupiter+20,yJupiter+20)
   #print("A tJ=", tJ, ", on a xGJupiter =", xJupiter+10, "et yGJupiter =", yJupiter+10)
   tJ+=1
   window.after(10,  animeJupiter)
   if tJ==360:
      tJ=0

# --- Saturne --- #

xSaturne, ySaturne, tS = miLEcran-9, miHEcran+113, 0
saturne = canvas.create_oval(xSaturne, ySaturne, xSaturne+18, ySaturne+18, fill='orange')
trajetoire = canvas.create_oval(miLEcran-122,miHEcran-122,miLEcran+122,miHEcran+122,outline='gray')


def animeSaturne():
   global xSaturne, ySaturne, tS
   angle = radians(tS)
   xSaturne = xSaturne + 2.1*cos(angle)
   ySaturne = ySaturne - 2.1*sin(angle)
   canvas.coords(saturne,xSaturne,ySaturne, xSaturne+18,ySaturne+18)
   #print("A tS=", tS, ", on a xGSaturne =", xSaturne+9, "et yGSaturne =", ySaturne+9)
   tS+=1
   window.after(10,  animeSaturne)
   if tS==360:
      tS=0

# --- Uranus --- #

xUranus, yUranus, tU = miLEcran-7, miHEcran+252, 0
uranus = canvas.create_oval(xUranus, yUranus, xUranus+14, yUranus+14, fill='blue')
trajetoire = canvas.create_oval(miLEcran-259,miHEcran-259,miLEcran+259,miHEcran+259,outline='gray')


def animeUranus():
   global xUranus, yUranus, tU
   angle = radians(tU)
   xUranus = xUranus + 4.45*cos(angle)
   yUranus = yUranus - 4.45*sin(angle)
   canvas.coords(uranus,xUranus,yUranus, xUranus+14,yUranus+14)
   #print("A tU=", tU, ", on a xGUranus =", xUranus+7, "et yGUranus =", yUranus+7)
   tU+=1
   window.after(10,  animeUranus)
   if tU==360:
      tU=0

# --- Neptune --- #

xNeptune, yNeptune, tN = miLEcran-7, miHEcran+398, 0
neptune = canvas.create_oval(xNeptune, yNeptune, xNeptune+14, yNeptune+14, fill='blue')
trajetoire = canvas.create_oval(miLEcran-405,miHEcran-405,miLEcran+405,miHEcran+405,outline='gray')


def animeNeptune():
   global xNeptune, yNeptune, tN
   angle = radians(tN)
   xNeptune = xNeptune + 7.07*cos(angle)
   yNeptune = yNeptune - 7.07*sin(angle)
   canvas.coords(neptune,xNeptune,yNeptune, xNeptune+14,yNeptune+14)
   #print("A tN=", tN, ", on a xGNeptune =", xNeptune+7, "et yGNeptune =", yNeptune+7)
   tN+=1
   window.after(10,  animeNeptune)
   if tN==360:
      tN=0

      
animeJupiter()
animeSaturne()
animeUranus()
animeNeptune()
window.mainloop



"""

--- Erreur ---
cosB, sinB = 0, 1
   co = (cosB + cos(angle))
   cosB = cos(angle)
   si = (sinB + sin(angle))
   sinB = sin(angle)
"""

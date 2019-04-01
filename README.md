# Basic-Programming
ITS320
import math
class Complex(object):
    def __init__(self, real, imaginary):
        
        self.real = real
        self.imaginary = imaginary
        
    def __add__(self, no):
        realadd = self.real + no.real # Add the real numbers
        imaginaryadd = self.imaginary + no.imaginary # Add the imaginary numbers
        return Complex(realadd, imaginaryadd) # Return results

    def __sub__(self, no):
        realsub = self.real - no.real # Subtract the real numbers
        imaginarysub = self.imaginary - no.imaginary # Subtract the imaginary numbers
        return Complex(realsub, imaginarysub) # Return results
    
    def __mul__(self, no):
        realmul = self.real * no.real # Multiply the real numbers
        imaginarymul = self.imaginary * no.imaginary # Multiply the imaginary numbers
        return Complex(realmul, imaginarymul) # Return results
    
    def __div__(self, no):
        realdiv = self.real / no.real # Divide the real numbers
        imaginarydiv = self.imaginary / no.imaginary # Divide the imaginary numbers
        return Complex(realdiv, imaginarydiv) # Return results

    def __mod__(self, no):
        realmod = self.real % no.real # Modulus of the real numbers
        imaginarymod = self.imaginary % no.imaginary # Modulus the imaginary numbers
        return Complex(realmod, imaginarymod) # Return results
    
def main_method():
    C = map(float, input().split())
    D = map(float, input().split())
    x = Complex(*C)
    y = Complex(*D)
    print = '\n'.join(map(str,[x+y,x-y,x*y,x/y,x.mod(),y.mod()]))

Complex(object)

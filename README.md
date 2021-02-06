# Formulas.py
#python program which contains functions, each of
which performs some intermediate task in the overall computation. 
#total of 4 functions that compute volume and surface area of certain 3-dimensional geometric figures

import math 

#sphere_volume(r) 
#computes the volume of a sphere of radius r by user 
def sphere_volume(r):
    a =(4/3)*(math.pi)*(r**3)
    return a
#end sphere_volume()

#sphere_area()
#computes surface area of a sphere with a given radius by user
def sphere_area(r):
    b =(4)*(math.pi)*(r**2)
    return b
#end sphere_area(r)

#cylinder_volume(r, h)
#computes volume of cylinder given r and h by user
def cylinder_volume(r, h):
    c =(math.pi)*(r**2)*(h)
    return c
#end cylinder_volume(r,h)

#cylinder_area(r, h)
#computes cylinder surface area given r and h by user 
def cylinder_area(r, h):
    d =(2)*(math.pi)*(r**2)+(2)*(math.pi)*(r)*(h)
    return d
#end cylinder_area(r,h)

#print_sphere(r) 
#prints a sphere's surface area and volume with 
#the instructions from previous functions
def print_sphere(r):
    print("The volume of the sphere with radius",str(r),"is:", sphere_volume(r))
    print("The surface area of the sphere with radius",str(r),"is:", sphere_area(r))
#end print_sphere(r)

#print_cylinder(r,h) 
#prints surface area and volume with
# the instructions from previous functions
def print_cylinder(r, h):
    print("The volume of the cylinder with radius",str(r),"and height",str(h),"is:", cylinder_volume(r,h))
    print("The surface area of the cylinder with radius",str(r),"and height",str(h),"is:", cylinder_area(r,h))
#end print_cylinder(r, h)

#-----------main program----------------------------------------------------
print("Enter three numbers:")
radius_string1 = input("first number: ")
radius_string2 = input("second number: ")
radius_string3 = input("third number: ")
print()

r = float(radius_string1)
print_sphere(r) 
print()

r = float(radius_string2)
print_sphere(r)
print()

r = float(radius_string3)
print_sphere(r)
print()

r = float(radius_string1)
h = float(radius_string2)
print_cylinder(r, h)
print()

r = float(radius_string2)
h = float(radius_string3)
print_cylinder(r, h)
print()

r = float(radius_string3)
h = float(radius_string1)
print_cylinder(r, h)
print()

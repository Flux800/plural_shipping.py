# plural_shipping.py
A parcel shipping startup.
```
weight = 4.8
#Ground Shipping
if weight <=2:
  cost_ground = weight * 1.50 + 20
elif weight >2 and weight <=6:
    cost_ground = weight * 3.00 + 20
elif weight >6 and weight <=10:
    cost_ground = weight * 4.00 + 20
else:
   cost_ground = weight * 4.75 + 20
print (cost_ground)

#Premium Ground Shipping
weght = 4.8
cost_pgs = 125.00
print (cost_pgs)

#Drone Shipping
weight = 4.8
if weight <=2:
  cost_drone = weight * 4.50
elif weight >2 and weight <=6:
    cost_drone = weight * 9.00
elif weight >6 and weight <=10:
    cost_drone = weight * 12.00
else:
   cost_drone = weight * 14.25
print (cost_drone)

# Compare costs
if cost_ground < cost_pgs and cost_ground < cost_drone:
    print("Ground shipping is cheapest: $", cost_ground)
elif cost_pgs < cost_ground and cost_pgs < cost_drone:
    print("Premium ground shipping is cheapest: $", cost_pgs)
else:
  print("Drone shipping is cheapest: $", cost_drone)
```

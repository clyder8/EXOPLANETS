# EXOPLANETS

import matplotlib.pyplot as plt
import numpy as np 





plt.figure(figsize=(7,12),dpi=900)
raidial_vel=(1,1,1,1,1,1,2,8,9,15,28,44,56,84,105,123,156,177,211,249,321,362,409,433,475,526,573,622,671,720,787,832,908,932)

transit=(0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,6,6,11,27,44,62,107,186,278,357,1158,2693,2782,3043,3147,3313,3728,3846)

imaging=(0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,5,6,7,8,8,8,8,9,9,10,10,10,14,14)

pulse_time=(0,0,0,2,2,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,4,4,4,4,4,6,6,6,6,6,6)

microlensning=(0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,1,3,3,5,6,6,6,7,8,8,9,9,9,9)

other=(0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,1,1,2,4,12,15,16,28,31,34,36,41,42,46,49)
plt.xlabel("Year. Starts at 1989")
plt.ylabel("discovered planets")
plt.title("EXOPLANET DETECTION METHODS")
plt.plot(raidial_vel,label="raidial velocity",color="green")
plt.plot(transit,label="transit method",color="black")
plt.plot(imaging,label="direct imaging",color="red")
plt.plot(pulse_time,label="pulsar timing",color="cyan")
plt.plot(microlensning,label="gravitatonal microlensing",color="purple")
plt.plot(other,label="other",color="blue")
plt.savefig("EXOPLANET DETECTION GRAPH", dpi = 400)
plt.legend()

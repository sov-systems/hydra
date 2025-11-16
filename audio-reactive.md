https://hydra.ojack.xyz/?code=YS5zZXRCaW5zKDEpJTIwJTJGJTJGJTIwYW1vdW50JTIwb2YlMjBiaW5zJTIwKGJhbmRzKSUyMHRvJTIwc2VwYXJhdGUlMjB0aGUlMjBhdWRpbyUyMHNwZWN0cnVtJTBBJTBBbm9pc2UoMiklMEElMDkubW9kdWxhdGUobzAlMkMoKSUzRCUzRWEuZmZ0JTVCMCU1RCowLjUpJTIwJTJGJTJGJTIwbGlzdGVuaW5nJTIwdG8lMjB0aGUlMjAybmQlMjBiYW5kJTBBJTA5Lm91dCgpJTBBJTBBYS5zZXRTbW9vdGgoLjEpJTIwJTJGJTJGJTIwYXVkaW8lMjByZWFjdGl2aXR5JTIwc21vb3RobmVzcyUyMGZyb20lMjAwJTIwdG8lMjAxJTJDJTIwdXNlcyUyMGxpbmVhciUyMGludGVycG9sYXRpb24lMEFhLnNldFNjYWxlKDgpJTIwJTIwJTIwJTIwJTJGJTJGJTIwbG91ZG5lc3MlMjB1cHBlciUyMGxpbWl0JTIwKG1hcHMlMjB0byUyMDApJTBBYS5zZXRDdXRvZmYoMC4xKSUyMCUyMCUyMCUyRiUyRiUyMGxvdWRuZXNzJTIwZnJvbSUyMHdoaWNoJTIwdG8lMjBzdGFydCUyMGxpc3RlbmluZyUyMHRvJTIwKG1hcHMlMjB0byUyMDApJTBBJTBBYS5zaG93KCklMjAlMkYlMkYlMjBzaG93JTIwd2hhdCUyMGh5ZHJhJ3MlMjBsaXN0ZW5pbmclMjB0byUwQSUyRiUyRmEuaGlkZSgpJTBBJTBBcmVuZGVyKG8wKQ%3D%3D

Use in conjunction with: https://phet.colorado.edu/sims/html/friction/latest/friction_all.html

Input device: BlackHole 2ch
Output device: Multi-Output Device

```
a.setBins(1) // amount of bins (bands) to separate the audio spectrum

noise(2)
	.modulate(o0,()=>a.fft[0]*0.5) // listening to the 2nd band
	.out()

a.setSmooth(.1) // audio reactivity smoothness from 0 to 1, uses linear interpolation
a.setScale(8)    // loudness upper limit (maps to 0)
a.setCutoff(0.1)   // loudness from which to start listening to (maps to 0)

a.show() // show what hydra's listening to
//a.hide()

render(o0)
```

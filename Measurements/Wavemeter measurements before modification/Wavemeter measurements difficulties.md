## Wavemeter measurements difficulties
While performing wavemeter measurements, on the VECSEL neXt just after getting it to run again, I encountered some difficulties.
Since the temperature of the case and therefore the GC were fluctuating so much, the VECSEL was very unstable in both frequency and power.
During a measurement, there were several times when the power dropped so mucht, that I couldn't change the exposure fast enough to get a sufficient signal on the wavemeter.
This lead to the wavemeter giving me a lot of readings that I couldn't interpret. The moment the power dropped below the threshold, the wavemeter would produce a wavelength reading of **-4 nm**.
Using this value, calculating an undisturbed Allan-deviation was not possible, since there would be huge jumps in frequency.

### Measurement on 21/05/2026
On this day I had the pump current at 20 A.

I managed to get a measurement of the frequency and only had the problem described above, occurring after around 500 seconds.\
<small>*I was informed later, that this measurement is normally only done for arround 3 min (180 seconds).*</small>

<img src="./fig/t_s_freq_21.05.2026,%2014.30,%20%20268,0945120%20THz.png" alt="Time series of frequency and power 21.05" width="1100"/>

Using the data from this measurement, I calculated the Allan-deviation, which is shown below for both the frequency and the power.

<img src="./fig/ad_freq_21.05.2026,%2014.30,%20%20268,0945120%20THz.png" alt="Allan-deviation of frequency 21.05" width="600"/>

<img src="./fig/ad_pow_21.05.2026,%2014.30,%20%20268,0945120%20THz.png" alt="Allan-deviation of power 21.05" width="600"/>

These plots show that the frequency stability for very short timescales (20 - 100 ms) is at around 30-50 MHz.\
Since they show an Allan-deviation, I would expect the deviation to drop for longer timescales before increasing again, but it only decreases for much higher timescales.\
This might be due to the constant frequency walking seen in the time series.
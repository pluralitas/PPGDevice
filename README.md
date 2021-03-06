# PPG Device using Arduino + PyQt5 GUI 

## Hardware
* Seeeduino Nano
http://wiki.seeedstudio.com/Seeeduino-Nano/
* Grove - Ear-clip Heart Rate Sensor http://wiki.seeedstudio.com/Grove-Ear-clip_Heart_Rate_Sensor/

![Seeeduino soldered to Prototype Board](https://lh3.googleusercontent.com/Fclw226I0LgYuIuTut3IVq9y9mrOh2Fb1ENM0ZXfhXKIZVxzj1Qq22IZB94BUh24WV2-QAf78hcQP2WP5xStJLVgcr94HjFMk6BaM-tcmkr2vSSAmJtbH7KCMge59Ad6v7aKueohPb4enP5HeIY9JCzd0atFeBXj3JFQUVK8fnoxPOaz01pYOU0c82-W1ciJIUoL53htLwPtqkkwoMOTAe3neaYCv1ozZ-AHhnd7tl1eXso8khuWYpyinyyRkPrW1YLb2bSJ90C8cqFsRj3ZSzsfYBWs0UpoyVXWfdVcfRKUcy6ILUOVUWErpYD4-7NsxjeIMrqKJ3FNe7BcQrqMTvDf2mjcccNvQMwGzraOPsEZPr3Ad5lGESdyGGWOTClGPZMEb8RXUmho2rhyzOHE4fe5DxW1f0w_Z-3kZxl5t9MPNYJG3VIdCRi29d3IrakRBMLypAAyluxtnEGecO1VUq5ulMFunWTLdMJ3CG5GQYXHYzxZmzMNU6irv6rpWdAl48-W-81nE5p5eYdy0ccjlg3pcZdeKzvvoYCLtKq31EJ4Eo9xBQwre4uXPD60gKSTxqNVHCyxy4DQXxfKrBrOXDkJYonPe10WNx1O7rW2G_63fY3Gp79iXd-QJTX9trzlOsf7da_2JEkx1y_E_6-9WwFvdPkwqjzx_dN29WlvCRu4GVncDgW4g1kRDJvlFw=w1274-h977-no)

![Grove PPG soldered to GND(Black), VCC(Red) and D2(Yellow) pin of Seeeduino Nano](https://lh3.googleusercontent.com/29idZc8UlDVgN1lhHFLRrJTpueOChUfp5llmSWRRbJusWdgfM6g8XBi1NnJhHAtk-F8pH3Le54ct2-KP3qPRi4o5-0ObJ2XYp9G3SDPfsSj5d30g3VbrmIKpXuUlKvSn00ENqDa_2fgPZOKpDn6AHM4y1F8jAl2aCCheC57zysH3LdlTUqvRjXNj_ZwqGEXZXT0ibG1mqYpQ4KWe0p9nekwYUGoQMaGDDVNEFyTmnprKv6MI3nzGWAUeHTaq9z7PhfkRZS5n8z-JbKYdBnifVqmM5dvqZr1kcRyFXRAQg6wluNbo8g06CjNto5O0i5OHmORlYIoArUMlm2xJ-LZ9rp6t0sxvVT4E3sPMuLCKIcAQwTtuXebb9luWuzdUwgsOpKnGMQ3Kcl99CShVXGdrI5jKNbC7HEIioTuCXDgrGaRESPIRg-5NN_tj5AUW4Bi7UGRyMa0M4LokmCeOy_yjOr3K91oSEpK_LGXFhoscOZUxhEILi8MOih6fYMWidfToBSTGewsedDxiOQ0lhmC7Ke4HL_511kwbEn1xbkDrdfvx5OQll5KYx7U1VtmljsRVaNVRFgrYaeTDyf5w2nz4cav6T4taTY1WgRaO2_3tRlXsHmuKScuQnNZSOcexHQlDNKMz0iwMcfEjp5wSwbgOI1WLUraKRnbgwxfbgfyAvPr4vdIhfP-QAyRvRKFuwQ=w1858-h914-no)

## Software
* Arduino code outputs time between each heartbeat to COM serial at 38400 baud
* Python version 3.6.10 64-bits
* QThread pyserial backend to read and calculate Heart Rate
* PyQt5 used for GUI front-end using pyqtSignal slots
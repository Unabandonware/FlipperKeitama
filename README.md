# FlipperKeitama
A collection of FlipperZero IR files that transmit items to the Keitai Kaitsuu! Tamagotchi Plus and Akai Version.

## About the Keitai Kaitsuu! Tamagotchi Plus (aka Keitama)
The Keitama is a Japan-exclusive Tamagotchi that was released as part of the Tamagotchi Connection series. This Tamagotchi was built to work with a companion mobile phone app called Tamagotchi Park (たまごっちパーク). The Tamagotchi Park app included various features, but its main purpose was to send items and gotchi points to the Keitama. The app generated 10-digit codes that could be inputted into the Keitama directly. These codes could also be sent through IR if you were using a compatible phone model.

# IR Transmission
To create the IR transmissions, the Tamagotchi Park app encoded the 10-digit codes into IR pulses through a scrambling and bit-reversal process. The full transmission protocol including pulse timings, bit order, and encoding process, was determined by examining the decompiled code from the Tamagotchi Park app.

# Passwords
The passwords were gathered from Curlour's [Neocities site](https://curlour.neocities.org/en/tmgc/ktama/listapw). Special thanks to Curlour for not only collecting these passwords, but also reverse engineering the algorithm that generates these passwords.

# How to Use
Navigate to the communication symbol (Heart symbol) and choose けいたい (Keitai) -> ゆうびん (Mail) -> つうしん (Communication). Line up the Keitama's IR port with the Flipper's IR port and beam the password.

Note: Some passwords will not work unless certain requirements have been fulfilled. For example, the parent passwords require to you have a matching tama from the previous generation and must be used in order. The Gotchi King code will only work if you have already donated 1000 Gotchi points. The hidden items and available travel tickets vary between the original Keitama and the Akai version. For more details, check out Curlour's [Neocities site](https://curlour.neocities.org/en/tmgc/ktama/listapw).

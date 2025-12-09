Implementation of S&H circuits

nmos S&H circuit

<img width="760" height="467" alt="Screenshot 2025-11-04 222215" src="https://github.com/user-attachments/assets/e9755893-ea34-4b69-8289-f5eb8a540107" />

L1=500n M to avoid Channel length modulation

W1=50u M

fin=10k Hz  , vdd=1.8 V

vin= 0.6 + 500 sin m V

vpulse= 0 to 1.8 V    Pulse width = 5u

CH(Hold capacitor) = 100p F



Output Waveform:


<img width="1268" height="562" alt="image" src="https://github.com/user-attachments/assets/7285921a-5186-4dff-a6bf-8564a53e1330" />

pmos S&H circuit


<img width="668" height="492" alt="image" src="https://github.com/user-attachments/assets/ae56eda1-7316-4b05-be78-876561454895" />


L1=500n M to avoid Channel length modulation

W1=50u M

fin=10k Hz        ,Vdd=1.8 V

vin= 1.25 + 500 sin m V

vpulse= 0 to 1.8 V     Pulse width = 5u

CH(Hold capacitor) = 100p F

Output Waveform :

<img width="1269" height="564" alt="image" src="https://github.com/user-attachments/assets/95127add-65fd-49f8-b6fc-4fc76072234c" />

cmos S&H circuit

<img width="675" height="474" alt="image" src="https://github.com/user-attachments/assets/8106b40a-bcad-4062-884e-080f46091b55" />

L1=500n M to avoid Channel length modulation

Wn=wp=50u M

fin=10k Hz    ,Vdd=1.8 V

vin= 1 + 500 sin m V

vpulse= 0 to 1.8 V     Pulse width = 5u

CH(Hold capacitor) = 100p F

Output Waveform:

<img width="1265" height="569" alt="image" src="https://github.com/user-attachments/assets/082d9b0f-6465-4736-a469-60e4afcf4ab2" />


Frequency Domain Analysis of CMOS S&H Circuit:

<img width="1590" height="670" alt="image" src="https://github.com/user-attachments/assets/7094720d-3f30-4de2-8c9f-8bae838b414d" />


Types of Sample and Hold architectures:

1) Open loop architecture:

<img width="821" height="315" alt="image" src="https://github.com/user-attachments/assets/67c59bfc-5579-480d-86fc-2b5567d21664" />


During tracking phase/ Acquisition mode, the transient current drawn from the input by CH can introduce noise at the input.So that input buffer is required to reduce this noise
The capacitor voltage during the hold mode can be affected by the current drawn by the following circuit. Therefore, the output voltage is buffered.
Buffer circuit at the input as well as at the output reduces the loading effect.
It will increases the complexity as well as non-idealities in the S/H circuit.


<img width="2431" height="1135" alt="image" src="https://github.com/user-attachments/assets/512845bd-6836-46c0-9a0c-d0b6b7dc7305" />


Design of Opamp(for Buffer)

<img width="504" height="279" alt="image" src="https://github.com/user-attachments/assets/9cea18b9-c10c-4258-961d-b2dcc53ce860" />

Design procedure

<img width="756" height="1045" alt="image" src="https://github.com/user-attachments/assets/11ec781a-dafa-4f3f-9679-6c698e617ada" />


<img width="581" height="613" alt="image" src="https://github.com/user-attachments/assets/b3194ce1-d56f-4afa-bda9-fd463f0e6c41" />


Test circuit

<img width="1889" height="1482" alt="image" src="https://github.com/user-attachments/assets/1a7aacbe-9bf0-4e05-886e-167cd4156f6f" />

AC analysis of opamp

<img width="3039" height="1370" alt="image" src="https://github.com/user-attachments/assets/5ab7b9e4-0bee-466d-88cc-0a756b219d69" />

Transient analysis of openloop S&H:

<img width="504" height="202" alt="image" src="https://github.com/user-attachments/assets/9ad9bb7a-7e19-4272-b398-0c24fefffe6d" />

Open loop S/H ckt  spectrum analysis

<img width="503" height="280" alt="image" src="https://github.com/user-attachments/assets/2343eefc-a6c6-4f03-bd9c-ead9e0025f68" />
















## Placement of ECG electrodes for acquiring the subject's cardiac electrical signal.
<img width="1514" height="646" alt="image" src="https://github.com/user-attachments/assets/f8b83b99-1846-4726-bb0b-e40803d74129" />

Electrode Placement for ECG Signal Acquisition

The image shows the placement of two ECG electrodes on the subject's body for acquiring the electrical activity of the heart. The electrodes are connected to the ECG sensor through wires.

The electrodes detect the small electrical potential differences produced by the heart during each cardiac cycle. Proper electrode placement and good skin contact are important for obtaining a clear ECG signal and reducing noise and motion artifacts.

After the electrodes are connected, the ECG sensor acquires the signal continuously. The acquired signal is then sent to the processing system, where it can be filtered, sampled, displayed as an ECG waveform, and further analyzed for the proposed robotic-vehicle control system.

## Real-time ECG signal acquired through serial communication and displayed on a computer.
<img width="1566" height="739" alt="image" src="https://github.com/user-attachments/assets/3c5a2323-644a-4823-9110-5a53b547eda8" />

The figure shows the ECG signal acquired from the subject and displayed on a computer through the serial communication (COM) interface. The waveform represents the electrical activity detected by the ECG electrodes.

After electrode placement and signal acquisition, the ECG sensor sends the analog signal to the processing/controller unit. The signal is sampled and transmitted to the computer, where the acquired data is displayed as a continuous waveform.

The displayed waveform contains variations corresponding to the cardiac electrical activity. In the initial acquisition stage, the signal may contain noise and fluctuations due to electrode contact, body movement, and other interference. The acquired data can subsequently be filtered and processed to obtain a cleaner ECG waveform.

## Real-Time ECG Signal Acquired Through Serial Communication
<img width="1583" height="768" alt="image" src="https://github.com/user-attachments/assets/3f59895d-00b8-4762-a39b-9c43e81c547e" />
The figure shows the ECG data being received through the COM port and displayed as a continuous waveform on the computer. The waveform contains fluctuations representing the acquired cardiac electrical signal. The variations seen in the waveform can also be influenced by noise and motion artifacts.

This raw acquired signal can be given to the next stage of the project for filtering, noise removal, feature extraction, and further analysis.
#Arduino Data Acquisition#
void setup()
{
    Serial.begin(9600);
}

void loop()
{
    int ecgData;

    ecgData = analogRead(A0);

    Serial.println(ecgData);

    delay(10);
}

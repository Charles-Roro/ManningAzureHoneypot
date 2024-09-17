1. Creating VM in Azure for Tracking Threat Activities.


![Screenshot 2024-09-17 at 12 22 14 AM](https://github.com/user-attachments/assets/30d9b9d2-b749-49ed-9898-37acd0f110c5)
![Screenshot 2024-09-17 at 12 23 12 AM](https://github.com/user-attachments/assets/d23c8ce6-2e5a-4689-a152-52262673ba10)
![Screenshot 2024-09-17 at 12 23 29 AM](https://github.com/user-attachments/assets/8d78735f-84b0-46a4-ab3b-804722c203cb)
![Screenshot 2024-09-17 at 12 26 56 AM](https://github.com/user-attachments/assets/86f5adb8-c806-48d4-9b87-e01c437512e0)

    Making a seperate security group with all ports open. This is to allow all traffic and pings to HIT the VM.
![Screenshot 2024-09-17 at 12 32 57 AM](https://github.com/user-attachments/assets/48e18729-0194-4b17-a0c9-8193936a24a7)
![Screenshot 2024-09-17 at 12 35 48 AM](https://github.com/user-attachments/assets/624cefed-3684-4fc4-8612-7a26ee222871)

    Creating a Log in Log Analytics workspace to make a Geolocation Log to track location of Threat Actors locations and IP's
![Screenshot 2024-09-17 at 12 42 26 AM](https://github.com/user-attachments/assets/bd34e365-38f7-48a0-9fab-0384fd9b92c9)

                Turning on Microsoft Defender to enable the ability to gather Logs. 
![Screenshot 2024-09-17 at 12 49 03 AM](https://github.com/user-attachments/assets/a06f5440-f35b-43cf-be6b-1b6aefedb3dd)
![Screenshot 2024-09-17 at 12 49 45 AM](https://github.com/user-attachments/assets/972cb266-76cd-4e33-a92e-67d20039e25f)

                    Connecting the Log to the created VM.
![Screenshot 2024-09-17 at 12 53 03 AM](https://github.com/user-attachments/assets/4f02ecc8-13fa-4d18-903c-0f54972d9997)
![Screenshot 2024-09-17 at 12 56 00 AM](https://github.com/user-attachments/assets/a9f53cb7-cb68-492b-8eee-7175aa63114c)


              Setting up Microsoft Sentinel to visualize the attack data
![Screenshot 2024-09-17 at 1 01 44 AM](https://github.com/user-attachments/assets/2af2c5e4-13fe-4fef-8fca-72f35abaef47)

      Logging in to the VM with Remote desktop to setup logging script and adjusting Firewall rules on the VM.
![Screenshot 2024-09-17 at 1 04 59 AM](https://github.com/user-attachments/assets/72f4602b-abf9-4b6b-933c-9dc931870897)

            Using Event Viewer in the VM to see failed Login attempts
![Screenshot 2024-09-17 at 1 17 52 AM](https://github.com/user-attachments/assets/496b91da-ac52-4e6c-906c-cb2d13d3bdf1)

        Pinging the VM on the main machine and setting up Firewall rules in the VM to allow attackers to find the VM faster through icmp echos
![Screenshot 2024-09-17 at 1 21 24 AM](https://github.com/user-attachments/assets/c796b62c-8337-47bb-9a7c-663f9cf56946)
![Screenshot 2024-09-17 at 1 26 25 AM](https://github.com/user-attachments/assets/e46a76d7-0f46-4e82-bd80-8e8ce421af3a)
![Screenshot 2024-09-17 at 1 29 28 AM](https://github.com/user-attachments/assets/d11dddb3-daf9-42de-86c5-2fe3300dd3f1)
![Screenshot 2024-09-17 at 1 30 03 AM](https://github.com/user-attachments/assets/b0c595a0-0c86-4da3-b3c0-d1416ceb7d74)
![Screenshot 2024-09-17 at 1 30 10 AM](https://github.com/user-attachments/assets/90738e8c-73fd-4fab-91fd-cf71816159f4)
                                              Pings now working 
![Screenshot 2024-09-17 at 1 31 27 AM](https://github.com/user-attachments/assets/a5ec0864-d3f2-4fe5-818c-3688e28c5dba)

                Using Powershell ISE to run the geolocation script
![Screenshot 2024-09-17 at 1 48 09 AM](https://github.com/user-attachments/assets/18f21237-eab9-4ef7-8bd0-612f6190d3c9)
          
              Script running and showing failed login attempts on the machine
![Screenshot 2024-09-17 at 1 51 18 AM](https://github.com/user-attachments/assets/2b446c95-bff6-45c1-8452-29f5f143adb5)

      Creating a custom Log in Log Analytics workspace to help Sentinel visualize the data
![Screenshot 2024-09-17 at 1 58 11 AM](https://github.com/user-attachments/assets/d8fa3d5c-4950-4950-bd57-b4c866d1afc1)
![Screenshot 2024-09-17 at 2 04 41 AM](https://github.com/user-attachments/assets/d437f5d8-545b-4fd3-ae72-81b13223e321)
![Screenshot 2024-09-17 at 2 06 05 AM](https://github.com/user-attachments/assets/1a32a1a1-1890-496b-81a4-0585406858b2)
![Screenshot 2024-09-17 at 2 06 31 AM](https://github.com/user-attachments/assets/7a7629ff-de11-450d-a616-cd8093eabf8f)




















































   

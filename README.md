# Texas-DPS-Appointment-Assistant
A simple python script help you get an earlier appointment at DPS in Texas ([Official Appointment Schdueling Website](https://public.txdpsscheduler.com/)).  

Supports three types of appointment: 
1. New Driver's License
2. Renew License
3. Road test

### What it does
* The script checks appointment availabilty in all DPS offices in Austin every one minute. 
* If you don't have any appointments, the script will found the earlist possible date and schedule it for you.
* If there is an available date earlier than your current appointment, the script will reschedule it for you.
* If a new appointment is rescheduled, you'll receive an email notifcation about the appointment details.


## requirements
python3 installed.

## Usage
|Service Type| type_id |
|-|-|
| Apply for first time Texas CLP/CDL | 71|
| Change, replace or renew Texas DL/Permit | 81 |
| Class C Road Skills Test |21|

1. replace the following line in [dps_check_availability.py](https://github.com/Ti-tanium/Texas-DPS-Appointment-Assistant/blob/0eb620007c119587f0f182f83e85b2f4efa5415f/dps_check_availability.py#L8-L13) with your information
```python
email = 'pushparajxa@gmail.com'
first_name = 'Pushparaj'
last_name = 'Motamari'
date_of_birth = '03/31/1989'
last4ssn = '9442'
zipcode = '75063'
type_id = 71 # service type id, 71 for new driver's license
```

2. in command line, run
```bash
python dps_check_availability.py
```

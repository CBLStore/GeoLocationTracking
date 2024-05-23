# GeoLocationTrack LWC
 
The GeoLocationTrack Lightning Web Component (LWC) is designed to enhance the functionality of the Salesforce platform by leveraging the device's geolocation capabilities. This component allows users to retrieve their current geographic location using GPS and update the corresponding <b> Internal SLR Geolocation </b> fields on a ServiceAppointment record in Salesforce. The component provides a user-friendly interface to fetch, display, and update location data seamlessly.
 
## Features
 
- Fetches the user's current location using the device's GPS.
- Displays the current location on a map.
- Updates the <b> Internal SLR Geolocation </b> fields of the ServiceAppointment record with the fetched location.
- Provides feedback via toast messages.

## Usage Scenario 
### Accessing the Service Appointment:
 Open the Salesforce FSL Mobile App on your mobile device. Then navigate to the list of Service Appointments assigned to you. select the specific Service Appointment you are currently working on.
<!-- <img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/0fb80cc3-a38b-43ac-b893-9034de73edae" width=360 height=800/><br>--> 

<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/1ae1ecf7-9a25-4db5-b0a8-295d677b8a4f" width=360 height=800/><br/>

### Opening the GeoLocation Component:
 Within the Service Appointment record page, navigate to the GeoLocation component embedded within the Action.

<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/7d00b12e-1dc6-4c31-b99c-3f2038c13417" width=360 height=800/><br/>

### Fetching the Current Location:
* The technician sees the component interface, which includes the "Get Current Location" and "Update Location" buttons.
* The technician taps the Get Current Location button.
* The component initiates a request to fetch the technician's current geolocation using the device's GPS.
  
<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/b8b2246d-3dfc-4392-86f4-cd907bb71228" width=360 height=400/><br>

### Displaying the Location:
- Once the location is successfully fetched, the component displays the latitude and longitude coordinates in text format.
- The technician also sees a map with a marker indicating their current location.
- A success toast message is displayed: "Location Detected: Location determined successfully."
  
<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/6071c483-71d4-43f5-aa3b-910b100023f6" width=360 height=800/><br/>

### Updating the Service Appointment Record:
- The technician verifies that the displayed location is accurate.
- They tap the Update Location button.
- The component updates the FSL__InternalSLRGeolocation__Latitude__s and FSL__InternalSLRGeolocation__Longitude__s fields of the Service Appointment record with the fetched coordinates.
- A success toast message is displayed: "Location Updated: Latitude and longitude fields updated successfully."
  
<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/70e41656-fb1b-4179-b895-a08160c7f6b3" width=360 height=800/><br>

### Confirming the Update:
- The technician receives confirmation that the Service Appointment record has been updated with the correct geolocation data.
- This updated information is now available for dispatchers and managers to view in real-time, ensuring accurate tracking and reporting.

<img src="https://github.com/CBLStore/GeoLocationTracking/assets/166477565/f314ae4c-8113-499b-917a-9d37e08148da" width=360 height=800/><br>





 

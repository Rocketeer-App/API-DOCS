# Key 

`=> API PUBLIC `  = Data shown in the public user api 

# User Database Schema 

**API ENTRY POINT:** `/user/{USERNAME}/KEY={API_KEY}`
<br><br>

`userId:` -> int   => **API PUBLIC**

`username: ` -> string => **API PUBLIC**

`password: ` -> sha256

`guilds: ` -> array => **API PUBLIC**

`friends: `-> array 

`joinDate: ` -> string => **API PUBLIC**

`isAdmin: ` -> boolean

`isSuspended: ` -> boolean

`isLoggedIn: ` -> boolean

`isBot: ` -> boolean => **API PUBLIC**

`premiumType: ` -> int => **API PUBLIC**

`email: ` -> string

`isVerified: ` -> boolean => **API PUBLIC**

`userSettings: ` -> array 

`profilePicture: ` -> string => **API PUBLIC**

`ownedApplications: ` -> array 
<br><br>


# User -> Guilds Database Model
**API ENTRY POINT:** `/guild/{ID}/KEY={API_KEY}`
<br><br>

`guildId: ` -> int => **API PUBLIC**

`guildIcon: ` -> string => **API PUBLIC**

`owner: ` -> string => **API PUBLIC**

`members: ` -> array => **API PUBLIC**

`requireVerification: ` -> boolean => **API PUBLIC**

`guildName: ` -> string => **API PUBLIC**

`guildMembers: ` -> array => **API PUBLIC**

`maxMembers: ` -> double ( Default: 20,000 ) 

`isNsfw: ` -> boolean => **API PUBLIC**

`premiumServerLevel: ` -> int => **API PUBLIC**
<br><br>

# User -> ownedApplications Database Model
**API ENTRY POINT:** `/application/{ID}/KEY={API_KEY}`
<br><br>

`appId: ` -> double => **API PUBLIC**

`appName: ` -> string => **API PUBLIC**

`profilePicture: ` -> string => **API PUBLIC**

`isPublic: ` -> boolean

`clientSecret` -> sha256 

`guilds: ` -> array => **API PUBLIC**

`owner: ` -> array => **API PUBLIC**


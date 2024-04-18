# My GitHub Profile

```python
class MyGitHubProfile:
    def __init__(self, name, username, location, bio, img_url, trophies, activity):
        self.name = name
        self.username = username
        self.location = location
        self.bio = bio
        self.img_url = img_url
        self.trophies = trophies
        self.activity = activity

    def display_profile(self):
        print(f"Name: {self.name}")
        print(f"Username: {self.username}")
        print(f"Location: {self.location}")
        print(f"Bio: {self.bio}")
        print(f"![Profile Image]({self.img_url})")
      
       

# Replace the placeholder values with your own information
profile = MyGitHubProfile(
    name="Deepanshu",
    username="deepanshu0211",
    location="India, Uttar pradesh",
    bio="I watch anime, h and i love playing Games ",
    img_url="https://i.pinimg.com/originals/1c/04/20/1c0420d2724872f9701aee8d2d064a77.gif",
    
   
)

profile.display_profile()

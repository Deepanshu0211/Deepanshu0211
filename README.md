
```python
class MyProfile:
    def __init__(self, name, username, location, bio, repositories, activity):
        self.name = name
        self.username = username
        self.location = location
        self.bio = bio
        self.repositories = repositories
        self.activity = activity

    def display_profile(self):
        print(f"Name: {self.name}")
        print(f"Username: {self.username}")
        print(f"Location: {self.location}")
        print(f"Bio: {self.bio}")
        print("\nRepositories:")
        for repo in self.repositories:
            print(f"- [{repo['name']}]({repo['url']})")
        print("\nRecent Activity:")
        for event in self.activity:
            print(f"- {event['type']}: {event['repo']} ({event['created_at']})")

# Replace the placeholder values with your own information
profile = MyProfile(
    name="Deepanshu",
    username="deepanshu0211",
    location="Uttar Pradesh",
    bio="I watch Anime and h and i love playing games ",
    repositories=[
        {"App Blocker": "Repository 1", "url": "https://github.com/Deepanshu0211/AppBlocker"},
        {"PortfollioTemplate": "Repository 2", "url": "https://github.com/Deepanshu0211/Portfollio-Template"},
        # Add more repositories as needed
    ],
    activity=[
        {"type": "PushEvent", "repo": "Repository 1", "created_at": "2024-04-18"},
        {"type": "IssueEvent", "repo": "Repository 2", "created_at": "2024-04-17"},
        # Add more activity events as needed
    ]
)

profile.display_profile()

import requests

ACCESS_TOKEN = "YOUR_ACCESS_TOKEN_HERE"  # Replace with your token
PAGE_ID = "YOUR_PAGE_ID_HERE"  # Replace with your Facebook Page ID
MESSAGE = "Hello, this is a test post from my Football Auto Bot!"

url = f"https://graph.facebook.com/{PAGE_ID}/feed"
data = {"message": MESSAGE, "access_token": ACCESS_TOKEN}

response = requests.post(url, data=data)
print(response.json())  # This will show the response from Facebook

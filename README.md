def greet_user():
    """Display a simple greeting."""
    print("Hello!")


greet_user()

def hello_world():
    """Display the famous hello world."""
    print("Hello World")


hello_world()


def greet_user(user):
    """Display a simple greeting."""
    print(f"Hello, {user.title()}!")

greet_user('matt')


def car_info(make, model):
    """Display vehicle info"""
    print(f"Here we have a {make.title()} {model.title()}!")

car_info('chevy', 'k1500')
car_info('chevy', 'c1500')
car_info('chevy', 'silverado')
car_info('chevy', 'volt')


def make_shirt(size, message):
     """Display vehicle info"""
     print(f"You have ordered a shirt!\nSIZE: {size.title()}\nMESSAGE: {message}!")

make_shirt('m', "I'm sleepy!")

def make_shirt(size='l', message= 'I love python'):
    """Display vehicle info"""
    print(f"You have ordered a shirt!\nSIZE: {size.title()}\nMESSAGE: {message}!")

make_shirt('m', "I'm sleepy!")
make_shirt()
make_shirt('m')
make_shirt('l', 'CTRL+C')
make_shirt('xxs', 'CTRL+V')

def describe_city(city, country):
    """Display city and country info"""
    print(f"{city.title()} is in {country}")


describe_city('Aiken', 'United States')
describe_city('Aiken', 'South Carolina')

#Make a function for an album
def get_formatted_album(album_name):
    """Return a full album name, neatly formatted."""
    album_name = f"\n {album_name} "
    return album_name.title()

name = get_formatted_album('What you see is what you get')
print(name)
#Make a function for an artist name
def get_artist_name(first_name, last_name):
    """Return a full name, neatly formatted."""
    full_name = f"{first_name} {last_name}"
    return full_name.title()

musician = get_artist_name('Luke', 'Combs')
print(musician)

#
Dict = {1: 'What you see is what you get', 2: 'This ones for you', 3: 'This one is for you too'}
print("\nDictionary with the use of Integer Keys to display album names: ")
print(Dict)

#Dictionary for artist name
def build_person(first_name, last_name, age=None):
    """Return a dictionary of information about that person"""
    person = {'first': first_name, 'last': last_name}
    if age:
        person['age'] = age
    return person

musician = build_person('luke', 'combs', age=31)
print(musician)

#Using a while loop
def make_album(artist_name, album_title, track= None):
    """Return a dictionary of information about an album and artist"""
    art = {'Artist': artist_name, 'Album': album_title}
    if track:
        art['Track'] = track
    return art

album = make_album('Luke Combs',"what you see is what you get", track = 8 )
album2 = make_album('Bon Jovi', "New Jersey", track = 14)
album3 = make_album('Survivior', "Rocky IV", track = 12)
album4 = make_album('AJR', "Ok Orchestra", track = 17)
print(f"\n{album}")
print(album2)
print(album3)
print(album4)

def get_user_albums(artist_name, album_title):
    """ users input"""
    art = f"{artist_name} {album_title}"
    return art  

while True:
    print("\nName your favorite artist and album by that artist.")
    print("(press 'q' to quit.)")
    artist_name = input("artist name: ")
    if artist_name == 'q':
        break
    album_name = input("album name: ")
    if album_name == 'q':
        break
    favorite_artist_album = get_user_albums(artist_name,album_name)
    print(f"Your favorite artist and album is {favorite_artist_album}.")



make_album(artist_name = None, album_title = None,)

while True:
    print("\nPlease tell me the album artist and title:")
    a_name = input("artist_name: ")
    al_name = input("album_name: ")

    artist_name = get_artist_name(a_name, al_name)
    print(f"\nThis is, {artist_name}!")

#Make a list showing a several short messages
def show_messages(messages):
 """Print simple short messages to the user"""
messages = ['\nHello', 'How are you', 'How is the family']
short_messages(messages)

#Write function called send_messages()
def send_messages(messages):
    """Print simple  message to the user"""
message = ['How are you', 'How are you doing','How is the family']
complete_messages = []
while message:
    current_messages = message.pop()
    print(f"\nPrinting model: {current_messages}")
    complete_messages.append(current_messages)
#Print both lists
print("\nThe messages have been printed:")
for complete_message in complete_messages:
        print(complete_message)


def send_messages():
    print("This function should print a message of both list")

    send_messages(messages)

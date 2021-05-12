# Dictionaries
#simple dictionary 
kkw = {'first_name': 'kim', 'last_name': 'kardashian', 'age' : 40, 'city': 'calabasas'}
print(kkw['first_name'])
print(kkw['last_name'])
print(kkw['age'])
print(kkw['city'])
print(kkw)

#adding values
kkw = {'spouse' : 'kanye'}
print(kkw)
print(f"\nKim Kardashian is married to {kkw['spouse']}.")

#removing values
print(kkw)
print(f"Kim Kardashian divorced {kkw['spouse']}.")
del kkw['spouse']
print(kkw)

#dictionalry using numbers
kuwk = {
    'kourtney' : 42,
    'kim' : 40,
    'khloe' : 36,
    'rob' : 34,
    'kendall' :25,
    'kylie' : 23,
}
ages = kuwk['kourtney']
print(f"\nKourtney Kardashian is {ages}.")
ages = kuwk['kim']
print(f"\nKim Kardashian is {ages}.")
ages = kuwk['khloe']
print(f"\nKhloe Kardashian is {ages}.")
ages = kuwk['rob']
print(f"\nRob Kardashian is {ages}.")
ages = kuwk['kendall']
print(f"\nKendall Jenner is {ages}.")
ages = kuwk['kylie']
print(f"\nKylie Jenner is {ages}.")

#empty dictionary
dash = {}
dash['mother'] = 'kris'
dash['status'] = 'not married'
print(dash)

#glossary example
weird_words = {
    'serendipity' : 'happy',
    'gobbledygook' : 'complicated',
    'scrumptious' : 'delishious',
    'jentacular' : 'breakfast',
    'xertz' : 'fast gulping'
}
meaning_1 = weird_words['serendipity'].title()
print(f"\nSerendipity means to be {meaning_1}.")

meaning_2 = weird_words['gobbledygook'].title()
print(f"\nGobbledygook means to be {meaning_2}.")

meaning_3 = weird_words['scrumptious'].title()
print(f"\nScrumptious means to be {meaning_3}.")

meaning_4 = weird_words['jentacular'].title()
print(f"\nJentacular means to be {meaning_4}.")

meaning_5 = weird_words['xertz'].title()
print(f"\nXertz means to be {meaning_5}.")

#river example
rivers_locations = {
    'nile' : 'egypt',
    'mississippi' : 'the united states',
    'amazon' : 'brazil',
}
    #.keys prints to the left of the colon of the dictionary; .value prints to the right of the colon of the dictionary
for river, location in rivers_locations.items():
    print(f"\nThe {river.title()} is in {location.title()}.")

print("\nThe following are the most famous rivers in the world:")
for river in rivers_locations.keys():
    print(river.title())

print("\nThe rivers are located in the following places around the world:")
for location in rivers_locations.values():
    print(location.title())


#Dictionary inside a dictionary
kim_k_husbands = []
for kim in kim_k_husbands:
    kim_k1 = {'damon thomas' :'2000 - 2004'}
    kim_k2 = {'kris humphries' : '2011 - 2013'}
    kim_k3 = {'kanye west' : '2014 - 2021'}
    kim_k_husbands.append(kim_k1)
for kim in kim_k_husbands[:1]:
    print(kim)
print("...")
print(f"\nKim's frost husband was in: {(kim_k_husbands)}")

kim_c1 = {'north' : 7}
kim_c2 = {'saint' : 5}
kim_c3 = {'chicago' : 3}
kim_c4 = {'psalm' : 2}
kim_k_children = [kim_c1, kim_c2, kim_c3, kim_c4]
for kim in kim_k_children:
    print(kim)

pet1 = {'dog': 'nacho', 'owner' : 'mark'}
pet2 = {'cat' : 'juno', 'owner' : 'dylan'}
pet3 = {'cat' : 'luna', 'owner' : 'erika'}
pet4 = {'cat' : 'frida', 'owner' : 'daniel'}
pets = [pet1, pet2, pet3, pet4]
for pet in pets:
    print(pet)

favorite_places = {
    'daniel' : ['whittier', 'mexico city'],
    'erika' : ['san francisco', 'los angeles'],
    'mark' : ['big bear', 'bolsa chica'],
    'dylan' : ['las vegas', 'west hollywood'],
}
for name, places in favorite_places.items() :
    print(f"\n{name.title()}'s favorite places are:")
    for place in places:
        print(f"\t{place.title()}")


cities = {
    'los angeles' : {
        'country': 'united states',
        'population' : 'four million',
        'fun fact' : 'hosted the Olympics twice',
    },
    'shanghai' : {
        'country': 'china',
        'population' : 'twenty six million',
        'fun fact' : 'largest city in the world',
    },
    'nairobi' : {
        'country': 'Kenya',
        'population' : 'four million',
        'fun fact' : 'served as a British provincial capital',
    },
}
for city, city_info in cities.items():
    print(f"\nCity: {city.title()}")
    country = f"{city_info['country']}"
    population = f"{city_info['population']}"
    fun_fact = city_info['fun fact']
    print(f"\tCountry: {country.title()}")
    print(f"\nPopulation: {population.lower()}")
    print(f"\nFun Fact: {fun_fact.lower()}")

# seleniumaws
import datetime
from faker import Faker
fake = Faker(locale='en_CA')

# ----------------- Moodle Web App DATA PARAMETERS ----------------------
app = 'Moodle'
moodle_url = 'http://52.39.5.126/'
moodle_home_page_title = 'Software Quality Assurance Testing'
moodle_login_page_url = 'http://52.39.5.126/login/index.php'
moodle_login_page_title = 'Software Quality Assurance Testing: Log in to the site'
moodle_dashboard_url = 'http://52.39.5.126/my/'
moodle_dashboard_title = 'Dashboard'
moodle_add_new_user_page_title = 'SQA: Administration: Users: Accounts: Add a new user'

admin_username = 'tkuser'
admin_password='Moodle!123'

new_username = fake.user_name()
new_password = fake.password()
first_name = fake.first_name()
last_name = fake.last_name()
email = fake.email()

moodle_net_profile = f'https://moodle.net/{new_username}'
city = fake.city()
country = fake.current_country()
description = f'User added by {admin_username} via Python Selenium Automated script on {datetime.datetime.now()}' # fake.sentence(nb_words=100)
# -----------------------------------------------------------------------

# dbdiagrams 

this tool helps you quickly generate beautiful database/ER diagrams for your postgres db schema :
- the script auto-generates the code by detecting postgres db schema
- this code can be then copy pasted onto an online tool called dbdiagram.io


### setup
required : python3

1. git clone https://github.com/nsingla/dbdiagrams.git

2. cd dbdiagrams

3. (optional) - use python virtual environment :
```bash
python -m venv env
source /env/bin/activate
```

4. install pre-requisite installation for psycopg2 (you could also install postgresql, otherwise libpq-dev and python-dev work):
```bash
sudo apt-get install libpq-dev python-dev 
pip install -r requirements.txt
```



### generating the code
- update the database connection string and output filepath in settings.conf
- run ./generate_code
- copy the generated code from the output file and visit dbdiagram.io [website](https://dbdiagram.io/d), once on the diagram page - paste it onto the code panel on the left. This should generate the diagram, make sure all the info is as desired - specially the references/table relationships. 
- you can screenshot the diagram and save image file or you can create an account if you like the tool (i've no affiliation) !

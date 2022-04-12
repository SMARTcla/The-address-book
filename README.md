In this homework, we will continue to develop our virtual assistant with a CLI interface.

Our assistant already knows how to interact with the user through the command line, receiving commands and arguments and performing the necessary actions. In this task, you will need to work on the internal logic of the assistant, on how data is stored, what kind of data and what can be done with it.

Let's apply object-oriented programming for these purposes. To begin with, we select several entities (models) with which we will work.

The user will have an address book or contact book. This contact book contains entries. Each record contains some set of fields.

Thus, we have described the entities (classes) that need to be implemented. Next, consider the requirements for these classes and establish their relationship, the rules by which they will interact.

The user interacts with the contact book by adding, deleting and editing entries. Also, the user should be able to search for records in the contact book by one or more criteria (fields).

You can also say about fields that they can be required (name) and optional (phone or email for example). Also records can contain several fields of the same type (several phones for example). The user should be able to add/delete/edit fields in any record.

For this homework, you should implement the following classes:

The AddressBook class, which inherits from UserDict, and we will then add the record search logic to this class.
The Record class, which is responsible for the logic of adding/removing/editing optional fields and storing the required Name field.
The Field class, which will be the parent for all fields, in which we then implement the logic common to all fields.
Class Name, a required field with a name.
The Phone class, an optional field with a phone number, and one record (Record) can contain several of them.
Admission Criteria#
All classes from the assignment are implemented.
Record entries in an AddressBook are stored as values ​​in a dictionary. The value Record.name.value is used as keys.
Record stores the Name object in a separate attribute.
Record stores a list of Phone objects in a separate attribute.
Record implements methods for adding/removing/editing Phone objects.
AddressBook implements the add_record method, which adds a Record to self.data.

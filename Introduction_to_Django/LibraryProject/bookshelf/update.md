# Update a Book
from bookshelf.models import Book

book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()

print(Book.objects.get(id=book.id).title)


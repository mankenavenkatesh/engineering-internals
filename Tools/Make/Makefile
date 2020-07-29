.DEFAULT_GOAL := generate

GREET_NAME = "venky"

say_hello: 
	@echo "Hello " ${GREET_NAME}

generate: 
	@echo "Creating empty files..."
	touch file-{1..10}.txt

clean:
	@echo "Cleaning up..."
	rm *.txt

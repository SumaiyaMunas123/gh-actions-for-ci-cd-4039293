PORT = 3000
NAME = python-api
PYTHON_VERSION = $(shell python3 --version | cut -d' ' -f2 | cut -d'.' -f1,2)
FMT  = black --check --diff *.py || true
LINT = flake8 --max-line-length=88 --ignore=E203,W503
TEST = python -m pytest --verbose --junit-xml=junit.xml
RUN  = uvicorn main:app --host 0.0.0.0 --port $(PORT) --reload

all: setup fmt lint test

setup: development
	pip install --requirement requirements.txt
	@echo "$(NAME) Application Setup complete"

development:
	pip install --upgrade pip
	pip install --requirement development-requirements.txt
	@echo "$(NAME) Development Setup complete"

fmt:
	$(FMT)

lint:
	$(LINT)

test:
	$(TEST)

run:
	$(RUN)

clean:
	@find . -type d -name "__pycache__" -exec rm -r {} + 2>/dev/null || true
	@find . -type f -name "*.pyc" -delete 2>/dev/null || true
	@find . -type f -name "*.pyo" -delete 2>/dev/null || true
	@find . -type f -name ".mypy_cache" -delete 2>/dev/null || true
	@find . -type d -name ".pytest_cache" -exec rm -r {} + 2>/dev/null || true
	@find . -type f -name "junit.xml" -delete 2>/dev/null || true
	@find . -type f -name ".coverage" -delete 2>/dev/null || true
	@find . -type d -name "htmlcov" -exec rm -r {} + 2>/dev/null || true
	@echo "Clean complete"

.PHONY: setup fmt lint test run clean all

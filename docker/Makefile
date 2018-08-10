NAME=ml
VERSION=1.0.0
IMAGE=originalgemlin/$(NAME)

build:
	docker build -t $(IMAGE) -t $(IMAGE):$(VERSION) .

run:
	docker run -it --rm --hostname $(NAME) --name $(NAME) \
		-p 8888:8888 \
		-v $(CURDIR)/data:/usr/local/ml/data \
		-v $(CURDIR)/..:/usr/local/ml/notebooks \
		-v $(CURDIR)/../..:/usr/local/dev \
		-v $(HOME)/.kaggle:/root/.kaggle \
		$(IMAGE):$(VERSION)

generate-api:
	oapi-codegen -package api api/api.yaml > api/api.gen.go

generate-mocks:
	go generate ./...

deps:
	go install github.com/deepmap/oapi-codegen/cmd/oapi-codegen@latest
	go install github.com/golang/mock/mockgen@v1.6.0

tests:
	go test -v ./...
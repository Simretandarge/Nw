# Use the desired Go version
FROM golang:1.24.2-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy all Go files into the container
COPY . .

# Install any dependencies (including Go modules)
RUN go mod tidy

# Build the Go application
RUN go build -o main .

# Expose the port the app will run on
EXPOSE 8082

# Run the application
CMD ["./main"]

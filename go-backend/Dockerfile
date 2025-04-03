# Use a specific Go version (e.g., 1.24.1)
FROM golang:1.24.1

# Set the working directory in the container
WORKDIR /app

# Copy all files from your local machine to the container
COPY . .

# Install dependencies (if required, run go mod tidy)
RUN go mod tidy

# Build the Go application
RUN go build -o main .

# Expose the port the app will run on
EXPOSE 8080

# Run the Go application
CMD ["./main"]

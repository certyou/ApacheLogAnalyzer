# Use a lightweight Python image
FROM python

# Set working directory
WORKDIR /app

# Copy files
COPY bytesOverTime.py ./
COPY requirements.txt ./

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Command to run script
CMD ["python", "bytesOverTime.py"]

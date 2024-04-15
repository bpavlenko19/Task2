# Task2
from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route('/register', methods=['POST'])
def register_user():
    
# Реалізація реєстрації користувача
    return jsonify({'message': 'User registered successfully'}), 201

if __name__ == '__main__':
    app.run(port=5001)

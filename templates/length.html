from flask import Flask, render_template, request

app = Flask(__name__)

# Conversion functions
def convert_length(value, from_unit, to_unit):
    conversion_factors = {
        'millimeter': 1,
        'centimeter': 10,
        'meter': 1000,
        'kilometer': 1e6,
        'inch': 25.4,
        'foot': 304.8,
        'yard': 914.4,
        'mile': 1.609e6
    }
    return value * conversion_factors[from_unit] / conversion_factors[to_unit]

def convert_weight(value, from_unit, to_unit):
    conversion_factors = {
        'milligram': 1,
        'gram': 1000,
        'kilogram': 1e6,
        'ounce': 28349.5,
        'pound': 453592
    }
    return value * conversion_factors[from_unit] / conversion_factors[to_unit]

def convert_temperature(value, from_unit, to_unit):
    if from_unit == 'Celsius':
        if to_unit == 'Fahrenheit':
            return value * 9/5 + 32
        elif to_unit == 'Kelvin':
            return value + 273.15
    elif from_unit == 'Fahrenheit':
        if to_unit == 'Celsius':
            return (value - 32) * 5/9
        elif to_unit == 'Kelvin':
            return (value - 32) * 5/9 + 273.15
    elif from_unit == 'Kelvin':
        if to_unit == 'Celsius':
            return value - 273.15
        elif to_unit == 'Fahrenheit':
            return (value - 273.15) * 9/5 + 32
    return value  # if from_unit and to_unit are the same

# Routes for different unit conversions
@app.route('/length', methods=['GET', 'POST'])
def length():
    if request.method == 'POST':
        value = float(request.form['value'])
        from_unit = request.form['from_unit']
        to_unit = request.form['to_unit']
        result = convert_length(value, from_unit, to_unit)
        return render_template('length.html', result=result)
    return render_template('length.html')

@app.route('/weight', methods=['GET', 'POST'])
def weight():
    if request.method == 'POST':
        value = float(request.form['value'])
        from_unit = request.form['from_unit']
        to_unit = request.form['to_unit']
        result = convert_weight(value, from_unit, to_unit)
        return render_template('weight.html', result=result)
    return render_template('weight.html')

@app.route('/temperature', methods=['GET', 'POST'])
def temperature():
    if request.method == 'POST':
        value = float(request.form['value'])
        from_unit = request.form['from_unit']
        to_unit = request.form['to_unit']
        result = convert_temperature(value, from_unit, to_unit)
        return render_template('temperature.html', result=result)
    return render_template('temperature.html')

if __name__ == '__main__':
    app.run(debug=True)

# Starting-Out-With-Python-Gaddis-3rd-ed
Starting Out With Python.  Gaddis, 3rd Edition

def main():
    loan_payment = get_loan_payment()
    insurance_payment = get_insurance_payment()
    gas = get_gas_expenses()
    oil = get_oil_expenses()
    tires = get_tire_expenses()
    maintainence = get_maintainence_expense()

    total_monthly_expenses = loan_payment  + insurance_payment + gas + oil \
                             + tires + maintainence
    print('Total Monthly Expenses: $', \
          format(total_monthly_expenses, ',.2f'), sep='')

    total_annual_expenses = total_monthly_expenses * 12
    print('Total Annual Expenses: $', \
          format(total_annual_expenses, ',.2f'), sep='')

def get_loan_payment():
    loan = float(input('Enter your monthly loan payment: '))
    return loan

def get_insurance_payment():
    insurance = float(input('Enter your monthly insurance payment: '))
    return insurance

def get_gas_expenses():
    gas = float(input('Enter your monthly gas expense: '))
    return gas

def get_oil_expenses():
    oil = float(input('Enter your monthly oil expense: '))
    return oil

def get_tire_expenses():
    tires = float(input('Enter your monthly tire expense: '))
    return tires

def get_maintainence_expense():
    maintainence = float(input('Enter your montly maintainence expense: '))
    return maintainence

main()

public class BankSystem {
    public static void main(String[] args) {
        System.out.println("Kumari Priya 079");
        System.out.println("______________________________________________");

        BankAccount regularAccount = new BankAccount("BA123", 500);
        regularAccount.deposit(1000);
        regularAccount.withdraw(600);

        System.out.println("______________________________________________");

        SavingsAccount savingsAccount = new SavingsAccount("SA1234", 450);
        savingsAccount.withdraw(300);

        System.out.println("______________________________________________");

        SavingsAccount anotherSavingsAccount = new SavingsAccount("SA1000", 300);
        anotherSavingsAccount.withdraw(250);
    }
}

class BankAccount {
    private String accountNumber;
    private double balance;
    private static int totalAccounts = 0;

    public BankAccount(String accountNumber, double balance) {
        this.accountNumber = accountNumber;
        this.balance = balance;
        totalAccounts++;
        System.out.println("Bank Account No.: " + accountNumber + "\nInitial balance: " + balance);
    }

    public void deposit(double amount) {
        System.out.println("Deposit of " + amount + " into account " + accountNumber);
        balance += amount;
        System.out.println("New balance after depositing " + amount + " is " + getBalance());
    }

    public void withdraw(double amount) {
        if (balance >= amount) {
            System.out.println("Withdrawing " + amount + " from account " + accountNumber);
            balance -= amount;
            System.out.println("New balance after withdrawing " + amount + " is " + getBalance());
        } else {
            System.out.println("Insufficient balance");
        }
    }

    public double getBalance() {
        return balance;
    }

    public static int getTotalAccounts() {
        return totalAccounts;
    }
}

class SavingsAccount extends BankAccount {
    public SavingsAccount(String accountNumber, double balance) {
        super(accountNumber, balance);
    }

    @Override
    public void withdraw(double amount) {
        if (getBalance() - amount < 100) {
            System.out.println("Minimum balance of at least 100 required");
        } else {
            super.withdraw(amount);
        }
    }
}

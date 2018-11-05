# java-project
@@ -56,10 +56,17 @@ public static void main(final String[] args) {
        sjp.run();
    }
     /**
     * Print the "Hello, world!" string.
     */
    public final void sayHello() {
        System.out.printf("Hello, %s!%n", name);
    }
     @Override
    public final void run() {
        do {
            System.out.printf("Hello, %s!%n", name);
            sayHello();
            try {
                Thread.sleep(PRINT_DELAY);
            } catch (InterruptedException e) {

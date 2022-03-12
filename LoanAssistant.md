/ *
* LoanAssistant.java
*/
package loanassistant;
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
public class LoanAssistant extends JFrame
{
public static void main(String args[])
{
// create frame
new LoanAssistant().show();
}
public LoanAssistant()
{
// frame constructor
setTitle("Loan Assistant");
setResizable(false);
addWindowListener(new WindowAdapter()
{
public void windowClosing(WindowEvent evt)
{
exitForm(evt);
}
});
getContentPane().setLayout(new GridBagLayout());
GridBagConstraints gridConstraints;
pack();
Dimension screenSize =
Toolkit.getDefaultToolkit().getScreenSize();
setBounds((int) (0.5 * (screenSize.width - getWidth())), (int) (0.5 * (screenSize.height
- getHeight())), getWidth(), getHeight());
}
private void exitForm(WindowEvent evt)
{
System.exit(0);
}
}

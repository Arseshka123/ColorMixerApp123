namespace ColorMixerApp123
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void numericRed_ValueChanged(object sender, EventArgs e)
        {
            int redValue = (int)numericRed.Value;
            int greenValue = 0;
            int blueValue = 0;

            redBox.BackColor = Color.FromArgb(redValue, greenValue, blueValue);
        }

        private void numericUpDown2_ValueChanged(object sender, EventArgs e)
        {
            int redValue = 0;
            int greenValue = (int)numericGreen.Value;
            int blueValue = 0;

            greenBox.BackColor = Color.FromArgb(redValue, greenValue, blueValue);
        }

        private void numericUpDown3_ValueChanged(object sender, EventArgs e)
        {

            int redValue = 0;
            int greenValue = 0;
            int blueValue = (int)numericBlue.Value;

            blueBox.BackColor = Color.FromArgb(redValue, greenValue, blueValue);
        }
    }
}

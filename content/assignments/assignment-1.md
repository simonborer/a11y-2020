---
title: "Assignment 1"
date: 2019-09-02T08:47:11+01:00
featured_image: hackers.gif
---
<div class="grid-container">
  <div class="grid-x grid-margin-x">
    <div class="cell small-10 small-offset-1">
      <div class="callout alert"><strong>Due Date</strong>: Before 4:59pm, Monday, September 30th</div>
      <p>Write SELECT statements to produce the required results.</p>
      <p>Your submitted assignment should be a well formatted SQL file.</p>
      <p>Use comments (lines in the file preceded by two hyphens to prevent their execution). Write your name, and the assignment number at the top of the file, and the question number above each query.</p>
      <p>Submit the assignment through Blackboard.</p>
      <section class="post-section">
        <h2>Questions</h2>
        <ol class="assignment__questions">
          <li>
            <ol>
              <li>Write a SELECT statement that returns three columns from the Vendors table: vendor_name, vendor_contact_last_name, and vendor_contact_first_name.</li>
              <li>Next, add code to this statement so it sorts the result set by last name and then first name.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns one column from the Vendors table named full_name. Create this column from the vendor_contact_first_name and vendor_contact_last_name columns, and format it like this: last name, comma, space, first name (for example, “Doe, John”).</li>
              <li>Next, sort the result set by last name and then first name.</li>
              <li>Then, filter the result set for contacts whose last name begins with the letter A, B, C, or E.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns four columns from the Invoices table named Due Date, Invoice Total, 10%, and Plus 10%. These columns should contain this data: 
                <ul>
                  <li><strong>Due Date</strong> The invoice_due_date column</li>
                  <li><strong>Invoice Total</strong> The invoice_total column</li>
                  <li><strong>10%</strong>10% of the value of invoice_total</li>
                  <li><strong>Plus 10%</strong> The value of invoice_total plus 10%</li>
                </ul>
                (For example, if invoice_total is 100, 10% is 10, and Plus 10% is 110)
              </li>
              <li>Next, filter the result set so it returns only those rows with an invoice total that’s greater than or equal to 500 and less than or equal to 1000.</li>
              <li>Then, sort the result set in descending sequence by invoice_due_date.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write and run a SELECT statement that returns four columns from the Invoices table named Number, Total, Credits, and Balance Due. These columns should include this data:
                <ul>
                  <li><strong>Number</strong> The invoice_number column</li>
                  <li><strong>Total</strong> The invoice_total column</li>
                  <li><strong>Credits</strong> Sum of the payment_total and credit_total columns</li>
                  <li><strong>Balance Due</strong> Invoice_total minus the sum of payment_total and credit_total</li>
                </ul>
              </li>
              <li>Next, filter for invoices with a balance due that’s greater than or equal to $500. Then, sort the result set by balance due in descending sequence.</li>
              <li>Finally, use another statement so the result set contains only the rows with the 10 largest balance dues.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns the balance due and the payment date from the Invoices table, but only when the payment_date column contains a null value.</li>
              <li>Then, modify the WHERE clause so it returns any invalid rows (rows in which the balance due is zero and the payment date is null).</li>
            </ol>
          </li>
          <li>Use the Dual table to create a row with these columns:
            <ul>
              <li><strong>Starting Principal</strong> Starting principle which should be equal to $51,000</li>
              <li><strong>New Principal</strong> Starting principal plus a 10% increase</li>
              <li><strong>Interest</strong> 6.5% of the new principal</li>
              <li><strong>Principal + Interest</strong> The new principal plus the interest (add the expression you used for the new principal calculation to the expression you used for the interest calculation)</li>
            </ul>
          </li>
          <li>Write a SELECT statement that returns all columns from the Vendors table inner-joined with all columns from the Invoices table.</li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns four columns:
                <table>
                  <thead>
                    <tr>
                      <th>Heading</th>
                      <th>Source</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td>vendor_name</td>
                      <td>vendor_name from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>invoice_number</td>
                      <td>invoice_number from the Invoices table</td>
                    </tr>
                    <tr>
                      <td>invoice_date</td>
                      <td>invoice_date from the Invoices table</td>
                    </tr>
                    <tr>
                      <td>balance_due</td>
                      <td>invoice_total minus payment_total minus credit_total from the Invoices table</td>
                    </tr>
                  </tbody>
                </table>
              </li>
              <li>The result set should have one row for each invoice with a non-zero balance.</li>
              <li>Sort the result set by vendor_name in ascending order.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns three columns:
                <table>
                  <thead>
                    <tr>
                      <th>Heading</th>
                      <th>Source</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td>vendor_name</td>
                      <td>vendor_name from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>default_account</td>
                      <td>default_account_number from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>description</td>
                      <td>account_description from the General_Ledger_Accounts table</td>
                    </tr>
                  </tbody>
                </table>
              </li>
              <li>The result set should have one row for each vendor, and it should be sorted by account_description and then by vendor_name.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns five columns:
                <table>
                  <thead>
                    <tr>
                      <th>Heading</th>
                      <th>Source</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td>vendor_name</td>
                      <td>vendor_name from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>invoice_date</td>
                      <td>invoice_date from the Invoices table</td>
                    </tr>
                    <tr>
                      <td>invoice_number</td>
                      <td>invoice_number from the Invoices table</td>
                    </tr>
                    <tr>
                      <td>li_sequence</td>
                      <td>invoice_sequence from the Invoice_Line_Items table</td>
                    </tr>
                    <tr>
                      <td>li_amount</td>
                      <td>line_item_amt from the Invoice_Line_Items table</td>
                    </tr>
                  </tbody>
                </table>
              </li>
              <li>Use these aliases for the tables: V for the Vendors table, I for the Invoices table, and LI for the Invoice_Line_Items table.</li>
              <li>Sort the final result set by vendor_name, invoice_date, invoice_number, and invoice_sequence.</li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns three columns:
                <table>
                  <thead>
                    <tr>
                      <th>Heading</th>
                      <th>Source</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td>vendor_id</td>
                      <td>vendor_id from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>vendor_name</td>
                      <td>vendor_name from the Vendors table</td>
                    </tr>
                    <tr>
                      <td>contact_name</td>
                      <td>A concatenation of vendor_contact_first_name and vendor_contact_last_name with a space in between</td>
                    </tr>
                  </tbody>
                </table>
              </li>
              <li>The result set should have one row for each vendor whose contact has the same last name as another vendor’s contact.</li>
              <li>The result set should be sorted by vendor_contact_last_name.</li>
              <li class="list-style-none"><em>Hint: what did we do in the lesson to find shared attributes in a table?</em></li>
            </ol>
          </li>
          <li>
            <ol>
              <li>Write a SELECT statement that returns two columns from the General_Ledger_Accounts table: account_number and account_description. </li>
              <li>The result set should have one row for each account number that has never been used or each value in the line_items table that has a NULL value.</li>
              <li>Sort the final result set by account_number.</li>
              <li class="list-style-none"><em>Hint: what other table might help you accomplish this?</em></li>
            </ol>
          </li>
        </ol>
      </section>
    </div>
  </div>
</div>

# Tugas18
Cypress Automation Test 
#negative login
describe('template spec', () => {
  it('login the internet', () => {
    cy.visit('https://the-internet.herokuapp.com/login')
    cy.get('#username').type('username')
    cy.get('#password').type('username')
    cy.get('.fa').click()
  })
})
#positif login
describe('template spec', () => {
  it('login the internet', () => {
    cy.visit('https://the-internet.herokuapp.com/login')
    cy.get('#username').type('tomsmith')
    cy.get('#password').type('SuperSecretPassword!')
    cy.get('.fa').click()
  })
})
